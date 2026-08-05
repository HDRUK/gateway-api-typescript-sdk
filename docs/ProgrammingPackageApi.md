# ProgrammingPackageApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createProgrammingPackages**](#createprogrammingpackages) | **POST** /api/v1/programming_packages | ProgrammingPackage@store|
|[**deleteProgrammingPackages**](#deleteprogrammingpackages) | **DELETE** /api/v1/programming_packages/{id} | ProgrammingPackage@destroy|
|[**editProgrammingPackages**](#editprogrammingpackages) | **PATCH** /api/v1/programming_packages/{id} | ProgrammingPackage@update|
|[**updateProgrammingPackages**](#updateprogrammingpackages) | **PUT** /api/v1/programming_packages/{id} | ProgrammingPackage@update|

# **createProgrammingPackages**
> CreateDarIntegration201Response createProgrammingPackages(createProgrammingLanguagesRequest)

Creates a new system programming package

### Example

```typescript
import {
    ProgrammingPackageApi,
    Configuration,
    CreateProgrammingLanguagesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingPackageApi(configuration);

let createProgrammingLanguagesRequest: CreateProgrammingLanguagesRequest; //Programming package definition

const { status, data } = await apiInstance.createProgrammingPackages(
    createProgrammingLanguagesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createProgrammingLanguagesRequest** | **CreateProgrammingLanguagesRequest**| Programming package definition | |


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

# **deleteProgrammingPackages**
> DeleteApplications200Response deleteProgrammingPackages()

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

# **editProgrammingPackages**
> UpdateProgrammingPackages200Response editProgrammingPackages(editProgrammingLanguagesRequest)

Edit a system programming package

### Example

```typescript
import {
    ProgrammingPackageApi,
    Configuration,
    EditProgrammingLanguagesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingPackageApi(configuration);

let id: number; //programming package id (default to undefined)
let editProgrammingLanguagesRequest: EditProgrammingLanguagesRequest; //ProgrammingPackage definition

const { status, data } = await apiInstance.editProgrammingPackages(
    id,
    editProgrammingLanguagesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editProgrammingLanguagesRequest** | **EditProgrammingLanguagesRequest**| ProgrammingPackage definition | |
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

# **updateProgrammingPackages**
> UpdateProgrammingPackages200Response updateProgrammingPackages(updateProgrammingLanguagesRequest)

Update a system programming package

### Example

```typescript
import {
    ProgrammingPackageApi,
    Configuration,
    UpdateProgrammingLanguagesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProgrammingPackageApi(configuration);

let id: number; //programming package id (default to undefined)
let updateProgrammingLanguagesRequest: UpdateProgrammingLanguagesRequest; //ProgrammingPackage definition

const { status, data } = await apiInstance.updateProgrammingPackages(
    id,
    updateProgrammingLanguagesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateProgrammingLanguagesRequest** | **UpdateProgrammingLanguagesRequest**| ProgrammingPackage definition | |
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

