# CategoryApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createCategories**](#createcategories) | **POST** /api/v1/categories | Category@store|
|[**deleteCategories**](#deletecategories) | **DELETE** /api/v1/categories/{id} | Category@destroy|
|[**editCategories**](#editcategories) | **PATCH** /api/v1/categories/{id} | Category@update|
|[**fetchAllCategories**](#fetchallcategories) | **GET** /api/v1/categories | Category@index|
|[**fetchCategories**](#fetchcategories) | **GET** /api/v1/categories/{id} | Category@show|
|[**updateCategories**](#updatecategories) | **PUT** /api/v1/categories/{id} | Category@update|

# **createCategories**
> CreateCategories200Response createCategories(createCategoriesRequest)

Creates a new tool category

### Example

```typescript
import {
    CategoryApi,
    Configuration,
    CreateCategoriesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CategoryApi(configuration);

let createCategoriesRequest: CreateCategoriesRequest; //Category definition

const { status, data } = await apiInstance.createCategories(
    createCategoriesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createCategoriesRequest** | **CreateCategoriesRequest**| Category definition | |


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

# **deleteCategories**
> DeleteAliases200Response deleteCategories()

Delete a tool category

### Example

```typescript
import {
    CategoryApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CategoryApi(configuration);

let id: number; //category id (default to undefined)

const { status, data } = await apiInstance.deleteCategories(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | category id | defaults to undefined|


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

# **editCategories**
> UpdateCategories200Response editCategories(editCategoriesRequest)

Edit a tool category

### Example

```typescript
import {
    CategoryApi,
    Configuration,
    EditCategoriesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CategoryApi(configuration);

let id: number; //category id (default to undefined)
let editCategoriesRequest: EditCategoriesRequest; //Category definition

const { status, data } = await apiInstance.editCategories(
    id,
    editCategoriesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editCategoriesRequest** | **EditCategoriesRequest**| Category definition | |
| **id** | [**number**] | category id | defaults to undefined|


### Return type

**UpdateCategories200Response**

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

# **fetchAllCategories**
> FetchAllCategories200Response fetchAllCategories()

Returns a list of categories enabled on the system

### Example

```typescript
import {
    CategoryApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CategoryApi(configuration);

let perPage: number; //per page (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllCategories(
    perPage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **perPage** | [**number**] | per page | (optional) defaults to undefined|


### Return type

**FetchAllCategories200Response**

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

# **fetchCategories**
> FetchAllCategories200Response fetchCategories()

Return a single tool category

### Example

```typescript
import {
    CategoryApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CategoryApi(configuration);

let id: number; //category id (default to undefined)

const { status, data } = await apiInstance.fetchCategories(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | category id | defaults to undefined|


### Return type

**FetchAllCategories200Response**

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

# **updateCategories**
> UpdateCategories200Response updateCategories(updateCategoriesRequest)

Update a tool category

### Example

```typescript
import {
    CategoryApi,
    Configuration,
    UpdateCategoriesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CategoryApi(configuration);

let id: number; //category id (default to undefined)
let updateCategoriesRequest: UpdateCategoriesRequest; //Category definition

const { status, data } = await apiInstance.updateCategories(
    id,
    updateCategoriesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateCategoriesRequest** | **UpdateCategoriesRequest**| Category definition | |
| **id** | [**number**] | category id | defaults to undefined|


### Return type

**UpdateCategories200Response**

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

