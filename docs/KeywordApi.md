# KeywordApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createKeywords**](#createkeywords) | **POST** /api/v1/keywords | KeywordController@store|
|[**deleteKeywords**](#deletekeywords) | **DELETE** /api/v1/keywords/{id} | KeywordController@destroy|
|[**editKeywords**](#editkeywords) | **PATCH** /api/v1/keywords/{id} | KeywordController@update|
|[**fetchAllKeywords**](#fetchallkeywords) | **GET** /api/v1/keywords | KeywordController@index|
|[**fetchKeywords**](#fetchkeywords) | **GET** /api/v1/keywords/{id} | KeywordController@show|
|[**updateKeywords**](#updatekeywords) | **PUT** /api/v1/keywords/{id} | KeywordController@update|

# **createKeywords**
> CreateCategories200Response createKeywords(createCategoriesRequest)

Creates a new keyword

### Example

```typescript
import {
    KeywordApi,
    Configuration,
    CreateCategoriesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new KeywordApi(configuration);

let createCategoriesRequest: CreateCategoriesRequest; //Keyword definition

const { status, data } = await apiInstance.createKeywords(
    createCategoriesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createCategoriesRequest** | **CreateCategoriesRequest**| Keyword definition | |


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
|**409** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteKeywords**
> DeleteAliases200Response deleteKeywords()

Delete a keyword by id

### Example

```typescript
import {
    KeywordApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new KeywordApi(configuration);

let id: number; //keyword id (default to undefined)

const { status, data } = await apiInstance.deleteKeywords(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | keyword id | defaults to undefined|


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

# **editKeywords**
> UpdateKeywords200Response editKeywords(editCategoriesRequest)

Edit a keyword by id

### Example

```typescript
import {
    KeywordApi,
    Configuration,
    EditCategoriesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new KeywordApi(configuration);

let id: number; //keyword id (default to undefined)
let editCategoriesRequest: EditCategoriesRequest; //Category definition

const { status, data } = await apiInstance.editKeywords(
    id,
    editCategoriesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editCategoriesRequest** | **EditCategoriesRequest**| Category definition | |
| **id** | [**number**] | keyword id | defaults to undefined|


### Return type

**UpdateKeywords200Response**

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

# **fetchAllKeywords**
> FetchAllKeywords200Response fetchAllKeywords()

Returns a list of keywords

### Example

```typescript
import {
    KeywordApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new KeywordApi(configuration);

let perPage: number; //Alternative output schema version. (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllKeywords(
    perPage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **perPage** | [**number**] | Alternative output schema version. | (optional) defaults to undefined|


### Return type

**FetchAllKeywords200Response**

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

# **fetchKeywords**
> FetchKeywords200Response fetchKeywords()

Return a single keyword

### Example

```typescript
import {
    KeywordApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new KeywordApi(configuration);

let id: number; //keyword id (default to undefined)

const { status, data } = await apiInstance.fetchKeywords(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | keyword id | defaults to undefined|


### Return type

**FetchKeywords200Response**

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

# **updateKeywords**
> UpdateKeywords200Response updateKeywords(updateCategoriesRequest)

Update a keyword by id

### Example

```typescript
import {
    KeywordApi,
    Configuration,
    UpdateCategoriesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new KeywordApi(configuration);

let id: number; //keyword id (default to undefined)
let updateCategoriesRequest: UpdateCategoriesRequest; //Keyword definition

const { status, data } = await apiInstance.updateKeywords(
    id,
    updateCategoriesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateCategoriesRequest** | **UpdateCategoriesRequest**| Keyword definition | |
| **id** | [**number**] | keyword id | defaults to undefined|


### Return type

**UpdateKeywords200Response**

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

