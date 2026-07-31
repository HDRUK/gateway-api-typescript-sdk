# DataAccessApplicationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createDarApplications**](#createdarapplications) | **POST** /api/v1/dar/applications | DataAccessApplication@store|
|[**deleteDarApplicationFiles**](#deletedarapplicationfiles) | **DELETE** /api/v1/dar/applications/{id}/files/{fileId} | DataAccessApplication@destroyFile|
|[**deleteDarApplications**](#deletedarapplications) | **DELETE** /api/v1/dar/applications/{id} | DataAccessApplication@destroy|
|[**deleteTeamDarApplicationFile**](#deleteteamdarapplicationfile) | **DELETE** /api/v1/teams/{teamId}/dar/applications/{id}/files/{fileId} | DataAccessApplication@destroyFile|
|[**deleteUserDarApplication**](#deleteuserdarapplication) | **DELETE** /api/v1/users/{userId}/dar/applications/{id} | DataAccessApplication@destroy|
|[**deleteUserDarApplicationFile**](#deleteuserdarapplicationfile) | **DELETE** /api/v1/users/{userId}/dar/applications/{id}/files/{fileId} | DataAccessApplication@destroyFile|
|[**fetchTeamDarApplicationAnswers**](#fetchteamdarapplicationanswers) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/answers | DataAccessApplication@showAnswers|
|[**fetchTeamDarApplicationDownloadZip**](#fetchteamdarapplicationdownloadzip) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/download | DataAccessApplication@download|
|[**fetchTeamDarApplicationFile**](#fetchteamdarapplicationfile) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/files/{fileId}/download | DataAccessApplication@downloadFile|
|[**fetchTeamDarApplicationFiles**](#fetchteamdarapplicationfiles) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/files | DataAccessApplication@showFiles|
|[**fetchTeamDarApplicationStatusHistory**](#fetchteamdarapplicationstatushistory) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/status | DataAccessApplication@status|
|[**fetchUserDarApplicationFile**](#fetchuserdarapplicationfile) | **GET** /api/v1/users/{userId}/dar/applications/{id}/files/{fileId}/download | DataAccessApplication@downloadFile|
|[**fetchUserDarApplicationFiles**](#fetchuserdarapplicationfiles) | **GET** /api/v1/users/{userId}/dar/applications/{id}/files | DataAccessApplication@showFiles|
|[**patchUserDarApplication**](#patchuserdarapplication) | **PATCH** /api/v1/users/{userId}/dar/applications/{id} | DataAccessApplication@update|
|[**updateTeamDarApplication**](#updateteamdarapplication) | **PATCH** /api/v1/teams/{teamId}/dar/applications/{id} | DataAccessApplication@update|
|[**updateUserDarApplication**](#updateuserdarapplication) | **PUT** /api/v1/users/{userId}/dar/applications/{id} | DataAccessApplication@update|

# **createDarApplications**
> CreateCategories200Response createDarApplications(createDarApplicationsRequest)

Creates a new DAR application

### Example

```typescript
import {
    DataAccessApplicationApi,
    Configuration,
    CreateDarApplicationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationApi(configuration);

let createDarApplicationsRequest: CreateDarApplicationsRequest; //DataAccessApplication definition

const { status, data } = await apiInstance.createDarApplications(
    createDarApplicationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createDarApplicationsRequest** | **CreateDarApplicationsRequest**| DataAccessApplication definition | |


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

# **deleteDarApplicationFiles**
> DeleteAliases200Response deleteDarApplicationFiles()

Delete a file associated with a DAR application

### Example

```typescript
import {
    DataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationApi(configuration);

let id: number; //DAR application id (default to undefined)
let fileId: string; //File id (default to undefined)

const { status, data } = await apiInstance.deleteDarApplicationFiles(
    id,
    fileId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DAR application id | defaults to undefined|
| **fileId** | [**string**] | File id | defaults to undefined|


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

# **deleteDarApplications**
> DeleteAliases200Response deleteDarApplications()

Delete a system DAR application

### Example

```typescript
import {
    DataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationApi(configuration);

let id: number; //DAR application id (default to undefined)

const { status, data } = await apiInstance.deleteDarApplications(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DAR application id | defaults to undefined|


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

# **deleteTeamDarApplicationFile**
> DeleteAliases200Response deleteTeamDarApplicationFile()

Delete a file associated with a DAR application

### Example

```typescript
import {
    DataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationApi(configuration);

let teamId: number; //Team id (default to undefined)
let id: number; //DAR application id (default to undefined)
let fileId: number; //File id (default to undefined)

const { status, data } = await apiInstance.deleteTeamDarApplicationFile(
    teamId,
    id,
    fileId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|
| **fileId** | [**number**] | File id | defaults to undefined|


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

# **deleteUserDarApplication**
> DeleteAliases200Response deleteUserDarApplication()

Delete a users DAR application

### Example

```typescript
import {
    DataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationApi(configuration);

let userId: number; //User id (default to undefined)
let id: number; //DAR application id (default to undefined)

const { status, data } = await apiInstance.deleteUserDarApplication(
    userId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | User id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|


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
|**401** | Unauthorized |  -  |
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteUserDarApplicationFile**
> DeleteAliases200Response deleteUserDarApplicationFile()

Delete a file associated with a DAR application

### Example

```typescript
import {
    DataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationApi(configuration);

let id: number; //DAR application id (default to undefined)
let userId: number; //User id (default to undefined)
let fileId: string; //File uuid (default to undefined)

const { status, data } = await apiInstance.deleteUserDarApplicationFile(
    id,
    userId,
    fileId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DAR application id | defaults to undefined|
| **userId** | [**number**] | User id | defaults to undefined|
| **fileId** | [**string**] | File uuid | defaults to undefined|


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

# **fetchTeamDarApplicationAnswers**
> FetchTeamDarApplicationAnswers200Response fetchTeamDarApplicationAnswers()

Return answers from a single DAR application

### Example

```typescript
import {
    DataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationApi(configuration);

let teamId: number; //Team id (default to undefined)
let id: number; //DAR application id (default to undefined)

const { status, data } = await apiInstance.fetchTeamDarApplicationAnswers(
    teamId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|


### Return type

**FetchTeamDarApplicationAnswers200Response**

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

# **fetchTeamDarApplicationDownloadZip**
> fetchTeamDarApplicationDownloadZip()

Returns a DAR form as a CSV with attached files as a zip

### Example

```typescript
import {
    DataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationApi(configuration);

let teamId: number; //Team id (default to undefined)
let id: number; //DAR application id (default to undefined)

const { status, data } = await apiInstance.fetchTeamDarApplicationDownloadZip(
    teamId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|


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

# **fetchTeamDarApplicationFile**
> fetchTeamDarApplicationFile()

Download a file associated with a DAR application

### Example

```typescript
import {
    DataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationApi(configuration);

let teamId: number; //Team id (default to undefined)
let id: number; //DAR application id (default to undefined)
let fileId: string; //File uuid (default to undefined)

const { status, data } = await apiInstance.fetchTeamDarApplicationFile(
    teamId,
    id,
    fileId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|
| **fileId** | [**string**] | File uuid | defaults to undefined|


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

# **fetchTeamDarApplicationFiles**
> FetchTeamDarApplicationFiles200Response fetchTeamDarApplicationFiles()

Return a list of files associated with a DAR application

### Example

```typescript
import {
    DataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationApi(configuration);

let teamId: number; //Team id (default to undefined)
let id: number; //DAR application id (default to undefined)

const { status, data } = await apiInstance.fetchTeamDarApplicationFiles(
    teamId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|


### Return type

**FetchTeamDarApplicationFiles200Response**

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

# **fetchTeamDarApplicationStatusHistory**
> FetchTeamDarApplicationStatusHistory200Response fetchTeamDarApplicationStatusHistory()

Return the status history of a single DAR application

### Example

```typescript
import {
    DataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationApi(configuration);

let teamId: number; //Team id (default to undefined)
let id: number; //DAR application id (default to undefined)

const { status, data } = await apiInstance.fetchTeamDarApplicationStatusHistory(
    teamId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|


### Return type

**FetchTeamDarApplicationStatusHistory200Response**

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

# **fetchUserDarApplicationFile**
> fetchUserDarApplicationFile()

Download a file associated with a DAR application

### Example

```typescript
import {
    DataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationApi(configuration);

let id: number; //DAR application id (default to undefined)
let userId: number; //User id (default to undefined)
let fileId: string; //File id (default to undefined)

const { status, data } = await apiInstance.fetchUserDarApplicationFile(
    id,
    userId,
    fileId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DAR application id | defaults to undefined|
| **userId** | [**number**] | User id | defaults to undefined|
| **fileId** | [**string**] | File id | defaults to undefined|


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

# **fetchUserDarApplicationFiles**
> FetchTeamDarApplicationFiles200Response fetchUserDarApplicationFiles()

Return a list of files associated with a DAR application

### Example

```typescript
import {
    DataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationApi(configuration);

let id: number; //DAR application id (default to undefined)
let userId: number; //User id (default to undefined)

const { status, data } = await apiInstance.fetchUserDarApplicationFiles(
    id,
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DAR application id | defaults to undefined|
| **userId** | [**number**] | User id | defaults to undefined|


### Return type

**FetchTeamDarApplicationFiles200Response**

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

# **patchUserDarApplication**
> FetchTeamDarApplication200Response patchUserDarApplication(patchUserDarApplicationRequest)

Edit a system DAR application

### Example

```typescript
import {
    DataAccessApplicationApi,
    Configuration,
    PatchUserDarApplicationRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationApi(configuration);

let userId: number; //User id (default to undefined)
let id: number; //DAR application id (default to undefined)
let patchUserDarApplicationRequest: PatchUserDarApplicationRequest; //DataAccessApplication definition

const { status, data } = await apiInstance.patchUserDarApplication(
    userId,
    id,
    patchUserDarApplicationRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **patchUserDarApplicationRequest** | **PatchUserDarApplicationRequest**| DataAccessApplication definition | |
| **userId** | [**number**] | User id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|


### Return type

**FetchTeamDarApplication200Response**

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

# **updateTeamDarApplication**
> FetchTeamDarApplication200Response updateTeamDarApplication(updateTeamDarApplicationRequest)

Edit a system DAR application

### Example

```typescript
import {
    DataAccessApplicationApi,
    Configuration,
    UpdateTeamDarApplicationRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationApi(configuration);

let teamId: number; //Team id (default to undefined)
let id: number; //DAR application id (default to undefined)
let updateTeamDarApplicationRequest: UpdateTeamDarApplicationRequest; //DataAccessApplication definition

const { status, data } = await apiInstance.updateTeamDarApplication(
    teamId,
    id,
    updateTeamDarApplicationRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateTeamDarApplicationRequest** | **UpdateTeamDarApplicationRequest**| DataAccessApplication definition | |
| **teamId** | [**number**] | Team id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|


### Return type

**FetchTeamDarApplication200Response**

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

# **updateUserDarApplication**
> FetchTeamDarApplication200Response updateUserDarApplication(updateUserDarApplicationRequest)

Update a system DAR application

### Example

```typescript
import {
    DataAccessApplicationApi,
    Configuration,
    UpdateUserDarApplicationRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationApi(configuration);

let userId: number; //User id (default to undefined)
let id: number; //DAR application id (default to undefined)
let updateUserDarApplicationRequest: UpdateUserDarApplicationRequest; //DataAccessApplication definition

const { status, data } = await apiInstance.updateUserDarApplication(
    userId,
    id,
    updateUserDarApplicationRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateUserDarApplicationRequest** | **UpdateUserDarApplicationRequest**| DataAccessApplication definition | |
| **userId** | [**number**] | User id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|


### Return type

**FetchTeamDarApplication200Response**

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

