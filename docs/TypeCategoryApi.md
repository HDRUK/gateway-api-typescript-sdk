# TypeCategoryApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createTypeCategories**](#createtypecategories) | **POST** /api/v1/type_categories | TypeCategory@store|
|[**deleteTypeCategories**](#deletetypecategories) | **DELETE** /api/v1/type_categories/{id} | TypeCategory@destroy|
|[**editTypeCategories**](#edittypecategories) | **PATCH** /api/v1/type_categories/{id} | TypeCategory@update|
|[**updateTypeCategories**](#updatetypecategories) | **PUT** /api/v1/type_categories/{id} | TypeCategory@update|

# **createTypeCategories**
> CreateDarIntegration201Response createTypeCategories(createTypeCategoriesRequest)

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

# **deleteTypeCategories**
> DeleteApplications200Response deleteTypeCategories()

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

# **editTypeCategories**
> UpdateTypeCategories200Response editTypeCategories(editProgrammingLanguagesRequest)

Edit a system type category

### Example

```typescript
import {
    TypeCategoryApi,
    Configuration,
    EditProgrammingLanguagesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TypeCategoryApi(configuration);

let id: number; //type category id (default to undefined)
let editProgrammingLanguagesRequest: EditProgrammingLanguagesRequest; //TypeCategory definition

const { status, data } = await apiInstance.editTypeCategories(
    id,
    editProgrammingLanguagesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editProgrammingLanguagesRequest** | **EditProgrammingLanguagesRequest**| TypeCategory definition | |
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

