# ProgrammingLanguageApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createProgrammingLanguages**](#createprogramminglanguages) | **POST** /api/v1/programming_languages | ProgrammingLanguage@store|
|[**deleteProgrammingLanguages**](#deleteprogramminglanguages) | **DELETE** /api/v1/programming_languages/{id} | ProgrammingLanguage@destroy|
|[**editProgrammingLanguages**](#editprogramminglanguages) | **PATCH** /api/v1/programming_languages/{id} | ProgrammingLanguage@update|
|[**updateProgrammingLanguages**](#updateprogramminglanguages) | **PUT** /api/v1/programming_languages/{id} | ProgrammingLanguage@update|

# **createProgrammingLanguages**
> CreateDarIntegration201Response createProgrammingLanguages(createProgrammingLanguagesRequest)

Creates a new system programming language

### Example

```typescript
import {
    ProgrammingLanguageApi,
    Configuration,
    CreateProgrammingLanguagesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingLanguageApi(configuration);

let createProgrammingLanguagesRequest: CreateProgrammingLanguagesRequest; //Programming language definition

const { status, data } = await apiInstance.createProgrammingLanguages(
    createProgrammingLanguagesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createProgrammingLanguagesRequest** | **CreateProgrammingLanguagesRequest**| Programming language definition | |


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

# **deleteProgrammingLanguages**
> DeleteApplications200Response deleteProgrammingLanguages()

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

# **editProgrammingLanguages**
> UpdateProgrammingLanguages200Response editProgrammingLanguages(editProgrammingLanguagesRequest)

Edit a system programming language

### Example

```typescript
import {
    ProgrammingLanguageApi,
    Configuration,
    EditProgrammingLanguagesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingLanguageApi(configuration);

let id: number; //programming language id (default to undefined)
let editProgrammingLanguagesRequest: EditProgrammingLanguagesRequest; //ProgrammingLanguage definition

const { status, data } = await apiInstance.editProgrammingLanguages(
    id,
    editProgrammingLanguagesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editProgrammingLanguagesRequest** | **EditProgrammingLanguagesRequest**| ProgrammingLanguage definition | |
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

# **updateProgrammingLanguages**
> UpdateProgrammingLanguages200Response updateProgrammingLanguages(updateProgrammingLanguagesRequest)

Update a system programming language

### Example

```typescript
import {
    ProgrammingLanguageApi,
    Configuration,
    UpdateProgrammingLanguagesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingLanguageApi(configuration);

let id: number; //programming language id (default to undefined)
let updateProgrammingLanguagesRequest: UpdateProgrammingLanguagesRequest; //ProgrammingLanguage definition

const { status, data } = await apiInstance.updateProgrammingLanguages(
    id,
    updateProgrammingLanguagesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateProgrammingLanguagesRequest** | **UpdateProgrammingLanguagesRequest**| ProgrammingLanguage definition | |
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

