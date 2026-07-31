# ProgrammingLanguageApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createProgrammingLanguages**](#createprogramminglanguages) | **POST** /api/v1/programming_languages | ProgrammingLanguage@store|
|[**deleteProgrammingLanguages**](#deleteprogramminglanguages) | **DELETE** /api/v1/programming_languages/{id} | ProgrammingLanguage@destroy|
|[**editProgrammingLanguages**](#editprogramminglanguages) | **PATCH** /api/v1/programming_languages/{id} | ProgrammingLanguage@update|
|[**fetchAllProgrammingLanguages**](#fetchallprogramminglanguages) | **GET** /api/v1/programming_languages | ProgrammingLanguage@index|
|[**fetchProgrammingLanguages**](#fetchprogramminglanguages) | **GET** /api/v1/programming_languages/{id} | ProgrammingLanguage@show|
|[**updateProgrammingLanguages**](#updateprogramminglanguages) | **PUT** /api/v1/programming_languages/{id} | ProgrammingLanguage@update|

# **createProgrammingLanguages**
> CreateCategories200Response createProgrammingLanguages(createCategoriesRequest)

Creates a new system programming language

### Example

```typescript
import {
    ProgrammingLanguageApi,
    Configuration,
    CreateCategoriesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingLanguageApi(configuration);

let createCategoriesRequest: CreateCategoriesRequest; //Programming language definition

const { status, data } = await apiInstance.createProgrammingLanguages(
    createCategoriesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createCategoriesRequest** | **CreateCategoriesRequest**| Programming language definition | |


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

# **deleteProgrammingLanguages**
> DeleteAliases200Response deleteProgrammingLanguages()

Delete a system programming language

### Example

```typescript
import {
    ProgrammingLanguageApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingLanguageApi(configuration);

let id: number; //programming language id (default to undefined)

const { status, data } = await apiInstance.deleteProgrammingLanguages(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | programming language id | defaults to undefined|


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

# **editProgrammingLanguages**
> UpdateProgrammingLanguages200Response editProgrammingLanguages(editCategoriesRequest)

Edit a system programming language

### Example

```typescript
import {
    ProgrammingLanguageApi,
    Configuration,
    EditCategoriesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingLanguageApi(configuration);

let id: number; //programming language id (default to undefined)
let editCategoriesRequest: EditCategoriesRequest; //ProgrammingLanguage definition

const { status, data } = await apiInstance.editProgrammingLanguages(
    id,
    editCategoriesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editCategoriesRequest** | **EditCategoriesRequest**| ProgrammingLanguage definition | |
| **id** | [**number**] | programming language id | defaults to undefined|


### Return type

**UpdateProgrammingLanguages200Response**

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

# **fetchAllProgrammingLanguages**
> FetchAllProgrammingLanguages200Response fetchAllProgrammingLanguages()

Returns a list of programming languages enabled on the system

### Example

```typescript
import {
    ProgrammingLanguageApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingLanguageApi(configuration);

const { status, data } = await apiInstance.fetchAllProgrammingLanguages();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**FetchAllProgrammingLanguages200Response**

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

# **fetchProgrammingLanguages**
> FetchProgrammingLanguages200Response fetchProgrammingLanguages()

Return a single system programming language

### Example

```typescript
import {
    ProgrammingLanguageApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingLanguageApi(configuration);

let id: number; //programming language id (default to undefined)

const { status, data } = await apiInstance.fetchProgrammingLanguages(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | programming language id | defaults to undefined|


### Return type

**FetchProgrammingLanguages200Response**

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

# **updateProgrammingLanguages**
> UpdateProgrammingLanguages200Response updateProgrammingLanguages(updateCategoriesRequest)

Update a system programming language

### Example

```typescript
import {
    ProgrammingLanguageApi,
    Configuration,
    UpdateCategoriesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingLanguageApi(configuration);

let id: number; //programming language id (default to undefined)
let updateCategoriesRequest: UpdateCategoriesRequest; //ProgrammingLanguage definition

const { status, data } = await apiInstance.updateProgrammingLanguages(
    id,
    updateCategoriesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateCategoriesRequest** | **UpdateCategoriesRequest**| ProgrammingLanguage definition | |
| **id** | [**number**] | programming language id | defaults to undefined|


### Return type

**UpdateProgrammingLanguages200Response**

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

