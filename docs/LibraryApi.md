# LibraryApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createLibraries**](#createlibraries) | **POST** /api/v1/libraries | Library@store|
|[**deleteLibraries**](#deletelibraries) | **DELETE** /api/v1/libraries/{id} | Library@destroy|
|[**editLibraries**](#editlibraries) | **PATCH** /api/v1/libraries/{id} | Library@update|
|[**fetchLibraries**](#fetchlibraries) | **GET** /api/v1/libraries/{id} | Return a single library|
|[**listLibraries**](#listlibraries) | **GET** /api/v1/libraries | Retrieve a list of libraries|
|[**updateLibraries**](#updatelibraries) | **PUT** /api/v1/libraries/{id} | Library@update|

# **createLibraries**
> CreateCategories200Response createLibraries(createLibrariesRequest)

Creates a new library

### Example

```typescript
import {
    LibraryApi,
    Configuration,
    CreateLibrariesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new LibraryApi(configuration);

let createLibrariesRequest: CreateLibrariesRequest; //library definition

const { status, data } = await apiInstance.createLibraries(
    createLibrariesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createLibrariesRequest** | **CreateLibrariesRequest**| library definition | |


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

# **deleteLibraries**
> DeleteAliases200Response deleteLibraries()

Delete a library

### Example

```typescript
import {
    LibraryApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new LibraryApi(configuration);

let id: number; //library id (default to undefined)

const { status, data } = await apiInstance.deleteLibraries(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | library id | defaults to undefined|


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

# **editLibraries**
> UpdateLibraries200Response editLibraries(createLibrariesRequest)

Edit a library

### Example

```typescript
import {
    LibraryApi,
    Configuration,
    CreateLibrariesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new LibraryApi(configuration);

let id: number; //library id (default to undefined)
let createLibrariesRequest: CreateLibrariesRequest; //library definition

const { status, data } = await apiInstance.editLibraries(
    id,
    createLibrariesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createLibrariesRequest** | **CreateLibrariesRequest**| library definition | |
| **id** | [**number**] | library id | defaults to undefined|


### Return type

**UpdateLibraries200Response**

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

# **fetchLibraries**
> FetchLibraries200Response fetchLibraries()

Return a single library

### Example

```typescript
import {
    LibraryApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new LibraryApi(configuration);

let id: number; //library id (default to undefined)

const { status, data } = await apiInstance.fetchLibraries(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | library id | defaults to undefined|


### Return type

**FetchLibraries200Response**

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

# **listLibraries**
> ListLibraries200Response listLibraries()

Returns a paginated list of libraries along with associated datasets and teams.

### Example

```typescript
import {
    LibraryApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new LibraryApi(configuration);

let perPage: number; //Specify the number of libraries per page (optional) (default to 10)

const { status, data } = await apiInstance.listLibraries(
    perPage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **perPage** | [**number**] | Specify the number of libraries per page | (optional) defaults to 10|


### Return type

**ListLibraries200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful operation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateLibraries**
> UpdateLibraries200Response updateLibraries(createLibrariesRequest)

Update a library

### Example

```typescript
import {
    LibraryApi,
    Configuration,
    CreateLibrariesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new LibraryApi(configuration);

let id: number; //library id (default to undefined)
let createLibrariesRequest: CreateLibrariesRequest; //library definition

const { status, data } = await apiInstance.updateLibraries(
    id,
    createLibrariesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createLibrariesRequest** | **CreateLibrariesRequest**| library definition | |
| **id** | [**number**] | library id | defaults to undefined|


### Return type

**UpdateLibraries200Response**

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

