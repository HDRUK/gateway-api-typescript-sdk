# AliasApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAliases**](#createaliases) | **POST** /api/v1/aliases | AliasController@store|
|[**deleteAliases**](#deletealiases) | **DELETE** /api/v1/aliases/{id} | AliasController@destroy|
|[**editAliases**](#editaliases) | **PATCH** /api/v1/aliases/{id} | AliasController@edit|
|[**fetchAliases**](#fetchaliases) | **GET** /api/v1/aliases/{id} | Return a single alias|
|[**fetchAllAliases**](#fetchallaliases) | **GET** /api/v1/aliases | List of aliases|
|[**updateAliases**](#updatealiases) | **PUT** /api/v1/aliases/{id} | AliasController@update|

# **createAliases**
> CreateAliases200Response createAliases(createAliasesRequest)

Creates a new alias

### Example

```typescript
import {
    AliasApi,
    Configuration,
    CreateAliasesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new AliasApi(configuration);

let createAliasesRequest: CreateAliasesRequest; //Alias definition

const { status, data } = await apiInstance.createAliases(
    createAliasesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createAliasesRequest** | **CreateAliasesRequest**| Alias definition | |


### Return type

**CreateAliases200Response**

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

# **deleteAliases**
> DeleteAliases200Response deleteAliases()

Delete an alias

### Example

```typescript
import {
    AliasApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new AliasApi(configuration);

let id: number; //alias id (default to undefined)

const { status, data } = await apiInstance.deleteAliases(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | alias id | defaults to undefined|


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

# **editAliases**
> UpdateAliases200Response editAliases(editAliasesRequest)

Edit a alias

### Example

```typescript
import {
    AliasApi,
    Configuration,
    EditAliasesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new AliasApi(configuration);

let id: number; //alias id (default to undefined)
let editAliasesRequest: EditAliasesRequest; //Alias definition

const { status, data } = await apiInstance.editAliases(
    id,
    editAliasesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editAliasesRequest** | **EditAliasesRequest**| Alias definition | |
| **id** | [**number**] | alias id | defaults to undefined|


### Return type

**UpdateAliases200Response**

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

# **fetchAliases**
> FetchAliases200Response fetchAliases()

Return a single alias

### Example

```typescript
import {
    AliasApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new AliasApi(configuration);

let id: number; //alias id (default to undefined)

const { status, data } = await apiInstance.fetchAliases(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | alias id | defaults to undefined|


### Return type

**FetchAliases200Response**

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

# **fetchAllAliases**
> FetchAllAliases200Response fetchAllAliases()

Returns a list of aliases

### Example

```typescript
import {
    AliasApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new AliasApi(configuration);

const { status, data } = await apiInstance.fetchAllAliases();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**FetchAllAliases200Response**

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

# **updateAliases**
> UpdateAliases200Response updateAliases(createAliasesRequest)

Update a alias

### Example

```typescript
import {
    AliasApi,
    Configuration,
    CreateAliasesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new AliasApi(configuration);

let id: number; //alias id (default to undefined)
let createAliasesRequest: CreateAliasesRequest; //Alias definition

const { status, data } = await apiInstance.updateAliases(
    id,
    createAliasesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createAliasesRequest** | **CreateAliasesRequest**| Alias definition | |
| **id** | [**number**] | alias id | defaults to undefined|


### Return type

**UpdateAliases200Response**

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

