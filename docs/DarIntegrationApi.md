# DarIntegrationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createDarIntegration**](#createdarintegration) | **POST** /api/v1/dar-integration/{id} | DarIntegration@store|
|[**deleteDarIntegration**](#deletedarintegration) | **DELETE** /api/v1/dar-integrations/{id} | DarIntegration@destroy|
|[**editDarIntegration**](#editdarintegration) | **PATCH** /api/v1/dar-integration/{id} | DarIntegration@edit|
|[**fetchAllDarIntegrations**](#fetchalldarintegrations) | **GET** /api/v1/dar-integration | DarIntegration@index|
|[**fetchDarIntegration**](#fetchdarintegration) | **GET** /api/v1/dar-integration/{id} | DarIntegration@show|
|[**updateDarIntegration**](#updatedarintegration) | **PUT** /api/v1/dar-integration/{id} | DarIntegration@update|

# **createDarIntegration**
> CreateDarIntegration201Response createDarIntegration(updateDarIntegrationRequest)

Creates a new DAR integration enabled on the system

### Example

```typescript
import {
    DarIntegrationApi,
    Configuration,
    UpdateDarIntegrationRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DarIntegrationApi(configuration);

let id: number; //dar integration id (default to undefined)
let updateDarIntegrationRequest: UpdateDarIntegrationRequest; //DarIntegration definition

const { status, data } = await apiInstance.createDarIntegration(
    id,
    updateDarIntegrationRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateDarIntegrationRequest** | **UpdateDarIntegrationRequest**| DarIntegration definition | |
| **id** | [**number**] | dar integration id | defaults to undefined|


### Return type

**CreateDarIntegration201Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Created |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteDarIntegration**
> DeleteApplications200Response deleteDarIntegration()

Delete a system Dar Integration

### Example

```typescript
import {
    DarIntegrationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DarIntegrationApi(configuration);

let id: number; //dar integration id (default to undefined)

const { status, data } = await apiInstance.deleteDarIntegration(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | dar integration id | defaults to undefined|


### Return type

**DeleteApplications200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**404** | Not found response |  -  |
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **editDarIntegration**
> UpdateDarIntegration200Response editDarIntegration(editDarIntegrationRequest)

Edit a DAR integration enabled on the system

### Example

```typescript
import {
    DarIntegrationApi,
    Configuration,
    EditDarIntegrationRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DarIntegrationApi(configuration);

let id: number; //dar integration id (default to undefined)
let editDarIntegrationRequest: EditDarIntegrationRequest; //DarIntegration definition

const { status, data } = await apiInstance.editDarIntegration(
    id,
    editDarIntegrationRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editDarIntegrationRequest** | **EditDarIntegrationRequest**| DarIntegration definition | |
| **id** | [**number**] | dar integration id | defaults to undefined|


### Return type

**UpdateDarIntegration200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Updated |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchAllDarIntegrations**
> FetchAllDarIntegrations200Response fetchAllDarIntegrations()

Returns a list of DAR integrations enabled on the system

### Example

```typescript
import {
    DarIntegrationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DarIntegrationApi(configuration);

const { status, data } = await apiInstance.fetchAllDarIntegrations();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**FetchAllDarIntegrations200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDarIntegration**
> FetchAllDarIntegrations200ResponseDataInner fetchDarIntegration()

Returns a single DAR integration enabled on the system

### Example

```typescript
import {
    DarIntegrationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DarIntegrationApi(configuration);

let id: number; //dar integration id (default to undefined)

const { status, data } = await apiInstance.fetchDarIntegration(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | dar integration id | defaults to undefined|


### Return type

**FetchAllDarIntegrations200ResponseDataInner**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**401** | Unauthorized |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateDarIntegration**
> UpdateDarIntegration200Response updateDarIntegration(updateDarIntegrationRequest)

Updates a DAR integration enabled on the system

### Example

```typescript
import {
    DarIntegrationApi,
    Configuration,
    UpdateDarIntegrationRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DarIntegrationApi(configuration);

let id: number; //dar integration id (default to undefined)
let updateDarIntegrationRequest: UpdateDarIntegrationRequest; //DarIntegration definition

const { status, data } = await apiInstance.updateDarIntegration(
    id,
    updateDarIntegrationRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateDarIntegrationRequest** | **UpdateDarIntegrationRequest**| DarIntegration definition | |
| **id** | [**number**] | dar integration id | defaults to undefined|


### Return type

**UpdateDarIntegration200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Updated |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

