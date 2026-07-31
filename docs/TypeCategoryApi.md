# TypeCategoryApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createTypeCategories**](#createtypecategories) | **POST** /api/v1/type_categories | TypeCategory@store|
|[**deleteTypeCategories**](#deletetypecategories) | **DELETE** /api/v1/type_categories/{id} | TypeCategory@destroy|
|[**editTypeCategories**](#edittypecategories) | **PATCH** /api/v1/type_categories/{id} | TypeCategory@update|
|[**fetchAllTypeCategories**](#fetchalltypecategories) | **GET** /api/v1/type_categories | TypeCategory@index|
|[**fetchTypeCategories**](#fetchtypecategories) | **GET** /api/v1/type_categories/{id} | TypeCategory@show|
|[**updateTypeCategories**](#updatetypecategories) | **PUT** /api/v1/type_categories/{id} | TypeCategory@update|

# **createTypeCategories**
> CreateCategories200Response createTypeCategories(createTypeCategoriesRequest)

Creates a new system type category

### Example

```typescript
import {
    TypeCategoryApi,
    Configuration,
    CreateTypeCategoriesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TypeCategoryApi(configuration);

let createTypeCategoriesRequest: CreateTypeCategoriesRequest; //Programming language definition

const { status, data } = await apiInstance.createTypeCategories(
    createTypeCategoriesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createTypeCategoriesRequest** | **CreateTypeCategoriesRequest**| Programming language definition | |


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

# **deleteTypeCategories**
> DeleteAliases200Response deleteTypeCategories()

Delete a system type category

### Example

```typescript
import {
    TypeCategoryApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TypeCategoryApi(configuration);

let id: number; //type category id (default to undefined)

const { status, data } = await apiInstance.deleteTypeCategories(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | type category id | defaults to undefined|


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

# **editTypeCategories**
> UpdateTypeCategories200Response editTypeCategories(editCategoriesRequest)

Edit a system type category

### Example

```typescript
import {
    TypeCategoryApi,
    Configuration,
    EditCategoriesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TypeCategoryApi(configuration);

let id: number; //type category id (default to undefined)
let editCategoriesRequest: EditCategoriesRequest; //TypeCategory definition

const { status, data } = await apiInstance.editTypeCategories(
    id,
    editCategoriesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editCategoriesRequest** | **EditCategoriesRequest**| TypeCategory definition | |
| **id** | [**number**] | type category id | defaults to undefined|


### Return type

**UpdateTypeCategories200Response**

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

# **fetchAllTypeCategories**
> FetchAllTypeCategories200Response fetchAllTypeCategories()

Returns a list of type categories enabled on the system

### Example

```typescript
import {
    TypeCategoryApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TypeCategoryApi(configuration);

const { status, data } = await apiInstance.fetchAllTypeCategories();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**FetchAllTypeCategories200Response**

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

# **fetchTypeCategories**
> FetchTypeCategories200Response fetchTypeCategories()

Return a single system type category

### Example

```typescript
import {
    TypeCategoryApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TypeCategoryApi(configuration);

let id: number; //type category id (default to undefined)

const { status, data } = await apiInstance.fetchTypeCategories(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | type category id | defaults to undefined|


### Return type

**FetchTypeCategories200Response**

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

# **updateTypeCategories**
> UpdateTypeCategories200Response updateTypeCategories(updateTypeCategoriesRequest)

Update a system type category

### Example

```typescript
import {
    TypeCategoryApi,
    Configuration,
    UpdateTypeCategoriesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TypeCategoryApi(configuration);

let id: number; //type category id (default to undefined)
let updateTypeCategoriesRequest: UpdateTypeCategoriesRequest; //TypeCategory definition

const { status, data } = await apiInstance.updateTypeCategories(
    id,
    updateTypeCategoriesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateTypeCategoriesRequest** | **UpdateTypeCategoriesRequest**| TypeCategory definition | |
| **id** | [**number**] | type category id | defaults to undefined|


### Return type

**UpdateTypeCategories200Response**

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

