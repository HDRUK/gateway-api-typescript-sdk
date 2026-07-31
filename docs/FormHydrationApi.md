# FormHydrationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getFormSchema**](#getformschema) | **GET** /api/v1/form_hydration/schema | Retrieve form schema data|
|[**onboardingFormHydration**](#onboardingformhydration) | **GET** /api/v1/form_hydration | Retrieve form schema data|

# **getFormSchema**
> object getFormSchema()

Retrieves form schema data based on the provided model and version.

### Example

```typescript
import {
    FormHydrationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new FormHydrationApi(configuration);

let model: string; //The model for which form schema is requested. (optional) (default to undefined)
let version: string; //The version of the model for which form schema is requested. (optional) (default to undefined)

const { status, data } = await apiInstance.getFormSchema(
    model,
    version
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **model** | [**string**] | The model for which form schema is requested. | (optional) defaults to undefined|
| **version** | [**string**] | The version of the model for which form schema is requested. | (optional) defaults to undefined|


### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful operation |  -  |
|**400** | Bad request. Missing required parameters or invalid parameters. |  -  |
|**500** | Internal server error. Failed to retrieve form schema data. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **onboardingFormHydration**
> object onboardingFormHydration()

Retrieves form schema data based on the provided model and version.

### Example

```typescript
import {
    FormHydrationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new FormHydrationApi(configuration);

let name: string; //The model name for which form schema is requested. (optional) (default to undefined)
let version: string; //The version of the model for which form schema is requested. (optional) (default to undefined)
let dataTypes: string; //The data types of the dataset about to be onboarded. (optional) (default to undefined)

const { status, data } = await apiInstance.onboardingFormHydration(
    name,
    version,
    dataTypes
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **name** | [**string**] | The model name for which form schema is requested. | (optional) defaults to undefined|
| **version** | [**string**] | The version of the model for which form schema is requested. | (optional) defaults to undefined|
| **dataTypes** | [**string**] | The data types of the dataset about to be onboarded. | (optional) defaults to undefined|


### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful operation |  -  |
|**400** | Bad request. Missing required parameters or invalid parameters. |  -  |
|**500** | Internal server error. Failed to retrieve form schema data. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

