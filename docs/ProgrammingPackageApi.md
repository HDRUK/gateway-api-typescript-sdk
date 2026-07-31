# ProgrammingPackageApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createProgrammingPackages**](#createprogrammingpackages) | **POST** /api/v1/programming_packages | ProgrammingPackage@store|
|[**deleteProgrammingPackages**](#deleteprogrammingpackages) | **DELETE** /api/v1/programming_packages/{id} | ProgrammingPackage@destroy|
|[**editProgrammingPackages**](#editprogrammingpackages) | **PATCH** /api/v1/programming_packages/{id} | ProgrammingPackage@update|
|[**fetchAllProgrammingPackages**](#fetchallprogrammingpackages) | **GET** /api/v1/programming_packages | ProgrammingPackage@index|
|[**fetchProgrammingPackages**](#fetchprogrammingpackages) | **GET** /api/v1/programming_packages/{id} | ProgrammingPackage@show|
|[**updateProgrammingPackages**](#updateprogrammingpackages) | **PUT** /api/v1/programming_packages/{id} | ProgrammingPackage@update|

# **createProgrammingPackages**
> CreateCategories200Response createProgrammingPackages(createCategoriesRequest)

Creates a new system programming package

### Example

```typescript
import {
    ProgrammingPackageApi,
    Configuration,
    CreateCategoriesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingPackageApi(configuration);

let createCategoriesRequest: CreateCategoriesRequest; //Programming package definition

const { status, data } = await apiInstance.createProgrammingPackages(
    createCategoriesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createCategoriesRequest** | **CreateCategoriesRequest**| Programming package definition | |


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

# **deleteProgrammingPackages**
> DeleteAliases200Response deleteProgrammingPackages()

Delete a system programming package

### Example

```typescript
import {
    ProgrammingPackageApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingPackageApi(configuration);

let id: number; //programming package id (default to undefined)

const { status, data } = await apiInstance.deleteProgrammingPackages(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | programming package id | defaults to undefined|


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

# **editProgrammingPackages**
> UpdateProgrammingPackages200Response editProgrammingPackages(editCategoriesRequest)

Edit a system programming package

### Example

```typescript
import {
    ProgrammingPackageApi,
    Configuration,
    EditCategoriesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingPackageApi(configuration);

let id: number; //programming package id (default to undefined)
let editCategoriesRequest: EditCategoriesRequest; //ProgrammingPackage definition

const { status, data } = await apiInstance.editProgrammingPackages(
    id,
    editCategoriesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editCategoriesRequest** | **EditCategoriesRequest**| ProgrammingPackage definition | |
| **id** | [**number**] | programming package id | defaults to undefined|


### Return type

**UpdateProgrammingPackages200Response**

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

# **fetchAllProgrammingPackages**
> FetchAllProgrammingPackages200Response fetchAllProgrammingPackages()

Returns a list of programming packages enabled on the system

### Example

```typescript
import {
    ProgrammingPackageApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingPackageApi(configuration);

const { status, data } = await apiInstance.fetchAllProgrammingPackages();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**FetchAllProgrammingPackages200Response**

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

# **fetchProgrammingPackages**
> FetchProgrammingPackages200Response fetchProgrammingPackages()

Return a single system programming package

### Example

```typescript
import {
    ProgrammingPackageApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingPackageApi(configuration);

let id: number; //programming package id (default to undefined)

const { status, data } = await apiInstance.fetchProgrammingPackages(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | programming package id | defaults to undefined|


### Return type

**FetchProgrammingPackages200Response**

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

# **updateProgrammingPackages**
> UpdateProgrammingPackages200Response updateProgrammingPackages(updateCategoriesRequest)

Update a system programming package

### Example

```typescript
import {
    ProgrammingPackageApi,
    Configuration,
    UpdateCategoriesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingPackageApi(configuration);

let id: number; //programming package id (default to undefined)
let updateCategoriesRequest: UpdateCategoriesRequest; //ProgrammingPackage definition

const { status, data } = await apiInstance.updateProgrammingPackages(
    id,
    updateCategoriesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateCategoriesRequest** | **UpdateCategoriesRequest**| ProgrammingPackage definition | |
| **id** | [**number**] | programming package id | defaults to undefined|


### Return type

**UpdateProgrammingPackages200Response**

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

