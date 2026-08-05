# DataAccessSectionApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createDarSection**](#createdarsection) | **POST** /api/v1/dar/sections | DataAccessSection@store|
|[**deleteDarSection**](#deletedarsection) | **DELETE** /api/v1/dar/sections/{id} | DataAccessSection@destroy|
|[**patchDarSection**](#patchdarsection) | **PATCH** /api/v1/dar/sections/{id} | DataAccessSection@update|
|[**updateDarSection**](#updatedarsection) | **PUT** /api/v1/dar/sections/{id} | DataAccessSection@update|

# **createDarSection**
> CreateDarIntegration201Response createDarSection(createDarSectionRequest)

Creates a new DAR section

### Example

```typescript
import {
    DataAccessSectionApi,
    Configuration,
    CreateDarSectionRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessSectionApi(configuration);

let createDarSectionRequest: CreateDarSectionRequest; //DataAccessSection definition

const { status, data } = await apiInstance.createDarSection(
    createDarSectionRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createDarSectionRequest** | **CreateDarSectionRequest**| DataAccessSection definition | |


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
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteDarSection**
> DeleteApplications200Response deleteDarSection()

Delete a system DAR section

### Example

```typescript
import {
    DataAccessSectionApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessSectionApi(configuration);

let id: number; //DAR section id (default to undefined)

const { status, data } = await apiInstance.deleteDarSection(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DAR section id | defaults to undefined|


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

# **patchDarSection**
> UpdateDarSection200Response patchDarSection(patchDarSectionRequest)

Edit a system DAR section

### Example

```typescript
import {
    DataAccessSectionApi,
    Configuration,
    PatchDarSectionRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessSectionApi(configuration);

let id: number; //DAR section id (default to undefined)
let patchDarSectionRequest: PatchDarSectionRequest; //DataAccessSection definition

const { status, data } = await apiInstance.patchDarSection(
    id,
    patchDarSectionRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **patchDarSectionRequest** | **PatchDarSectionRequest**| DataAccessSection definition | |
| **id** | [**number**] | DAR section id | defaults to undefined|


### Return type

**UpdateDarSection200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**404** | Not found response |  -  |
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateDarSection**
> UpdateDarSection200Response updateDarSection(createDarSectionRequest)

Update a system DAR section

### Example

```typescript
import {
    DataAccessSectionApi,
    Configuration,
    CreateDarSectionRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessSectionApi(configuration);

let id: number; //DAR section id (default to undefined)
let createDarSectionRequest: CreateDarSectionRequest; //DataAccessSection definition

const { status, data } = await apiInstance.updateDarSection(
    id,
    createDarSectionRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createDarSectionRequest** | **CreateDarSectionRequest**| DataAccessSection definition | |
| **id** | [**number**] | DAR section id | defaults to undefined|


### Return type

**UpdateDarSection200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**404** | Not found response |  -  |
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

