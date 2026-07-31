# DataAccessTemplateApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createDarTemplate**](#createdartemplate) | **POST** /api/v1/dar/templates | DataAccessTemplate@store|
|[**deleteDarTemplate**](#deletedartemplate) | **DELETE** /api/v1/dar/templates/{id} | DataAccessTemplate@destroy|
|[**downloadDarTemplateFile**](#downloaddartemplatefile) | **GET** /api/v1/dar/templates/{id}/download | DataAccessTemplate@downloadFile|
|[**fetchDarTemplate**](#fetchdartemplate) | **GET** /api/v1/dar/templates/{id} | DataAccessTemplate@show|
|[**fetchDarTemplates**](#fetchdartemplates) | **GET** /api/v1/dar/templates | DataAccessTemplate@index|
|[**patchDarTemplate**](#patchdartemplate) | **PATCH** /api/v1/dar/templates/{id} | DataAccessTemplate@update|
|[**updateDarTemplate**](#updatedartemplate) | **PUT** /api/v1/dar/templates/{id} | DataAccessTemplate@update|

# **createDarTemplate**
> CreateCategories200Response createDarTemplate(createDarTemplateRequest)

Creates a new DAR template

### Example

```typescript
import {
    DataAccessTemplateApi,
    Configuration,
    CreateDarTemplateRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessTemplateApi(configuration);

let createDarTemplateRequest: CreateDarTemplateRequest; //DataAccessTemplate definition

const { status, data } = await apiInstance.createDarTemplate(
    createDarTemplateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createDarTemplateRequest** | **CreateDarTemplateRequest**| DataAccessTemplate definition | |


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

# **deleteDarTemplate**
> DeleteAliases200Response deleteDarTemplate()

Delete a system DAR template

### Example

```typescript
import {
    DataAccessTemplateApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessTemplateApi(configuration);

let id: number; //DAR template id (default to undefined)

const { status, data } = await apiInstance.deleteDarTemplate(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DAR template id | defaults to undefined|


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

# **downloadDarTemplateFile**
> downloadDarTemplateFile()

Download the template for a file based DAR application

### Example

```typescript
import {
    DataAccessTemplateApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessTemplateApi(configuration);

let id: number; //DAR template id (default to undefined)

const { status, data } = await apiInstance.downloadDarTemplateFile(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DAR template id | defaults to undefined|


### Return type

void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: file, application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDarTemplate**
> FetchDarTemplate200Response fetchDarTemplate()

Return a single DAR template

### Example

```typescript
import {
    DataAccessTemplateApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessTemplateApi(configuration);

let id: number; //DAR template id (default to undefined)

const { status, data } = await apiInstance.fetchDarTemplate(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DAR template id | defaults to undefined|


### Return type

**FetchDarTemplate200Response**

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

# **fetchDarTemplates**
> FetchDarTemplates200Response fetchDarTemplates()

List of DAR templates

### Example

```typescript
import {
    DataAccessTemplateApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessTemplateApi(configuration);

let withQuestions: number; //Include questions in response (optional) (default to undefined)
let published: string; //Template publication status to filter by (true, false) (optional) (default to undefined)

const { status, data } = await apiInstance.fetchDarTemplates(
    withQuestions,
    published
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **withQuestions** | [**number**] | Include questions in response | (optional) defaults to undefined|
| **published** | [**string**] | Template publication status to filter by (true, false) | (optional) defaults to undefined|


### Return type

**FetchDarTemplates200Response**

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

# **patchDarTemplate**
> PatchDarTemplate200Response patchDarTemplate(patchDarTemplateRequest)

Edit a system DAR template

### Example

```typescript
import {
    DataAccessTemplateApi,
    Configuration,
    PatchDarTemplateRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessTemplateApi(configuration);

let id: number; //DAR template id (default to undefined)
let patchDarTemplateRequest: PatchDarTemplateRequest; //DataAccessTemplate definition
let sectionId: number; //Section id (optional) (default to undefined)

const { status, data } = await apiInstance.patchDarTemplate(
    id,
    patchDarTemplateRequest,
    sectionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **patchDarTemplateRequest** | **PatchDarTemplateRequest**| DataAccessTemplate definition | |
| **id** | [**number**] | DAR template id | defaults to undefined|
| **sectionId** | [**number**] | Section id | (optional) defaults to undefined|


### Return type

**PatchDarTemplate200Response**

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

# **updateDarTemplate**
> FetchDarTemplate200Response updateDarTemplate(updateDarTemplateRequest)

Update a system DAR template

### Example

```typescript
import {
    DataAccessTemplateApi,
    Configuration,
    UpdateDarTemplateRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessTemplateApi(configuration);

let id: number; //DAR template id (default to undefined)
let updateDarTemplateRequest: UpdateDarTemplateRequest; //DataAccessTemplate definition

const { status, data } = await apiInstance.updateDarTemplate(
    id,
    updateDarTemplateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateDarTemplateRequest** | **UpdateDarTemplateRequest**| DataAccessTemplate definition | |
| **id** | [**number**] | DAR template id | defaults to undefined|


### Return type

**FetchDarTemplate200Response**

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

