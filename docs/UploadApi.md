# UploadApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createFiles**](#createfiles) | **POST** /api/v1/files | Upload@upload|
|[**deleteFilesProcessed**](#deletefilesprocessed) | **DELETE** /api/v1/files/processed/{id} | Upload@destroy|
|[**fetchFiles**](#fetchfiles) | **GET** /api/v1/files/{uuid} | Upload@show|
|[**fetchFilesProcessedContent**](#fetchfilesprocessedcontent) | **GET** /api/v1/files/processed/{uuid}/download | Upload@content|

# **createFiles**
> CreateFiles200Response createFiles()

Upload a file to the gateway-api via scanning sub-service

### Example

```typescript
import {
    UploadApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UploadApi(configuration);

let entityFlag: string; //Flag to indicate the purpose of the file upload e.g. dur-from-upload (optional) (default to undefined)
let teamId: number; //Id of team associated with the file upload (optional) (default to undefined)
let applicationId: number; //Id of dar application associated with the file upload (optional) (default to undefined)
let questionId: number; //Id of the question in the dar application associated with the file upload (optional) (default to undefined)

const { status, data } = await apiInstance.createFiles(
    entityFlag,
    teamId,
    applicationId,
    questionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **entityFlag** | [**string**] | Flag to indicate the purpose of the file upload e.g. dur-from-upload | (optional) defaults to undefined|
| **teamId** | [**number**] | Id of team associated with the file upload | (optional) defaults to undefined|
| **applicationId** | [**number**] | Id of dar application associated with the file upload | (optional) defaults to undefined|
| **questionId** | [**number**] | Id of the question in the dar application associated with the file upload | (optional) defaults to undefined|


### Return type

**CreateFiles200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Upload complete |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteFilesProcessed**
> DeleteAliases200Response deleteFilesProcessed()

Delete a processed file

### Example

```typescript
import {
    UploadApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UploadApi(configuration);

let id: string; //file uuid (default to undefined)

const { status, data } = await apiInstance.deleteFilesProcessed(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | file uuid | defaults to undefined|


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

# **fetchFiles**
> FetchFiles200Response fetchFiles()

Get the scanning status of an upload

### Example

```typescript
import {
    UploadApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UploadApi(configuration);

let uuid: string; //upload id (default to undefined)

const { status, data } = await apiInstance.fetchFiles(
    uuid
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **uuid** | [**string**] | upload id | defaults to undefined|


### Return type

**FetchFiles200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchFilesProcessedContent**
> FetchFilesProcessedContent200Response fetchFilesProcessedContent()

Get the content of a processed file

### Example

```typescript
import {
    UploadApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UploadApi(configuration);

let uuid: string; //upload id (default to undefined)

const { status, data } = await apiInstance.fetchFilesProcessedContent(
    uuid
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **uuid** | [**string**] | upload id | defaults to undefined|


### Return type

**FetchFilesProcessedContent200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

