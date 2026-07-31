# DataAccessSectionApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createDarSection**](#createdarsection) | **POST** /api/v1/dar/sections | DataAccessSection@store|
|[**deleteDarSection**](#deletedarsection) | **DELETE** /api/v1/dar/sections/{id} | DataAccessSection@destroy|
|[**fetchDarSection**](#fetchdarsection) | **GET** /api/v1/dar/sections/{id} | DataAccessSection@show|
|[**fetchDarSections**](#fetchdarsections) | **GET** /api/v1/dar/sections | DataAccessSection@index|
|[**patchDarSection**](#patchdarsection) | **PATCH** /api/v1/dar/sections/{id} | DataAccessSection@update|
|[**updateDarSection**](#updatedarsection) | **PUT** /api/v1/dar/sections/{id} | DataAccessSection@update|

# **createDarSection**
> CreateCategories200Response createDarSection(createDarSectionRequest)

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

**CreateCategories200Response**

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
> DeleteAliases200Response deleteDarSection()

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

**DeleteAliases200Response**

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

# **fetchDarSection**
> FetchDarSection200Response fetchDarSection()

Return a single DAR section

### Example

```typescript
import {
    DataAccessSectionApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessSectionApi(configuration);

let id: number; //DAR section id (default to undefined)

const { status, data } = await apiInstance.fetchDarSection(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DAR section id | defaults to undefined|


### Return type

**FetchDarSection200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDarSections**
> FetchDarSections200Response fetchDarSections()

List of DAR sections

### Example

```typescript
import {
    DataAccessSectionApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessSectionApi(configuration);

let perPage: number; //per page (optional) (default to undefined)

const { status, data } = await apiInstance.fetchDarSections(
    perPage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **perPage** | [**number**] | per page | (optional) defaults to undefined|


### Return type

**FetchDarSections200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patchDarSection**
> FetchDarSection200Response patchDarSection(patchDarSectionRequest)

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

**FetchDarSection200Response**

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
> FetchDarSection200Response updateDarSection(createDarSectionRequest)

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

**FetchDarSection200Response**

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

