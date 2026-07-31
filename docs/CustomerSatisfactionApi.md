# CustomerSatisfactionApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createCsat**](#createcsat) | **POST** /api/v1/csat | Create Customer Satisfaction Score|
|[**editCsat**](#editcsat) | **PATCH** /api/v1/csat/{id} | Update Customer Satisfaction Description|

# **createCsat**
> DeleteAliases200Response createCsat(createCsatRequest)

Creates a customer satisfaction score between 0 and 5

### Example

```typescript
import {
    CustomerSatisfactionApi,
    Configuration,
    CreateCsatRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustomerSatisfactionApi(configuration);

let createCsatRequest: CreateCsatRequest; //Customer Satisfaction score

const { status, data } = await apiInstance.createCsat(
    createCsatRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createCsatRequest** | **CreateCsatRequest**| Customer Satisfaction score | |


### Return type

**DeleteAliases200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Resource Created |  -  |
|**422** | Validation Error |  -  |
|**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **editCsat**
> EditCsat200Response editCsat(editCsatRequest)

Update a description for a satisfaction score entry

### Example

```typescript
import {
    CustomerSatisfactionApi,
    Configuration,
    EditCsatRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustomerSatisfactionApi(configuration);

let id: number; //ID of the CSAT entry (default to undefined)
let editCsatRequest: EditCsatRequest; //Reason to update

const { status, data } = await apiInstance.editCsat(
    id,
    editCsatRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editCsatRequest** | **EditCsatRequest**| Reason to update | |
| **id** | [**number**] | ID of the CSAT entry | defaults to undefined|


### Return type

**EditCsat200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Update successful |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

