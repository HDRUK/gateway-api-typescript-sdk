# ApplicationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createApplications**](#createapplications) | **POST** /api/v1/applications | ApplicationController@store|
|[**deleteApplications**](#deleteapplications) | **DELETE** /api/v1/applications/{id} | ApplicationController@delete|
|[**editApplications**](#editapplications) | **PATCH** /api/v1/applications/{id} | ApplicationController@edit|
|[**fetchAllApplications**](#fetchallapplications) | **GET** /api/v1/applications | ApplicationController@index|
|[**fetchAllSitemap**](#fetchallsitemap) | **GET** /api/v1/sitemap | SiteMapController@index|
|[**fetchApplications**](#fetchapplications) | **GET** /api/v1/applications/{id} | ApplicationController@show|
|[**patchApplicationsClientId**](#patchapplicationsclientid) | **PATCH** /api/v1/applications/{id}/clientid | ApplicationController@generateClientIdById|
|[**updateApplications**](#updateapplications) | **PUT** /api/v1/applications/{id} | ApplicationController@update|

# **createApplications**
> CreateApplications200Response createApplications(createApplicationsRequest)

Creates application

### Example

```typescript
import {
    ApplicationApi,
    Configuration,
    CreateApplicationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ApplicationApi(configuration);

let createApplicationsRequest: CreateApplicationsRequest; //Application definition

const { status, data } = await apiInstance.createApplications(
    createApplicationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createApplicationsRequest** | **CreateApplicationsRequest**| Application definition | |


### Return type

**CreateApplications200Response**

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

# **deleteApplications**
> DeleteApplications200Response deleteApplications()

Delete application

### Example

```typescript
import {
    ApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ApplicationApi(configuration);

let id: number; //application id (default to undefined)

const { status, data } = await apiInstance.deleteApplications(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | application id | defaults to undefined|


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

# **editApplications**
> UpdateApplications200Response editApplications(editApplicationsRequest)

Edit application

### Example

```typescript
import {
    ApplicationApi,
    Configuration,
    EditApplicationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ApplicationApi(configuration);

let id: number; //application id (default to undefined)
let editApplicationsRequest: EditApplicationsRequest; //ActivityLog definition

const { status, data } = await apiInstance.editApplications(
    id,
    editApplicationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editApplicationsRequest** | **EditApplicationsRequest**| ActivityLog definition | |
| **id** | [**number**] | application id | defaults to undefined|


### Return type

**UpdateApplications200Response**

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

# **fetchAllApplications**
> FetchAllApplications200Response fetchAllApplications()

Returns a list of applications

### Example

```typescript
import {
    ApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ApplicationApi(configuration);

let teamId: number; //Filter Apps by the teamId (optional) (default to undefined)
let text: string; //Search term to filter by application name or description. (optional) (default to undefined)
let status: '1' | '0'; //Filter by application status is enabled or not (true or false). (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllApplications(
    teamId,
    text,
    status
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Filter Apps by the teamId | (optional) defaults to undefined|
| **text** | [**string**] | Search term to filter by application name or description. | (optional) defaults to undefined|
| **status** | [**&#39;1&#39; | &#39;0&#39;**]**Array<&#39;1&#39; &#124; &#39;0&#39;>** | Filter by application status is enabled or not (true or false). | (optional) defaults to undefined|


### Return type

**FetchAllApplications200Response**

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

# **fetchAllSitemap**
> FetchAllSitemap200Response fetchAllSitemap()

Returns a list of all ids and last updated date for Collections, Data Custodians, Data Custodian Networks, Durs, DataSets, Tools

### Example

```typescript
import {
    ApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ApplicationApi(configuration);

const { status, data } = await apiInstance.fetchAllSitemap();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**FetchAllSitemap200Response**

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

# **fetchApplications**
> FetchApplications200Response fetchApplications()

Get application by id

### Example

```typescript
import {
    ApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ApplicationApi(configuration);

let id: number; //application id (default to undefined)

const { status, data } = await apiInstance.fetchApplications(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | application id | defaults to undefined|


### Return type

**FetchApplications200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patchApplicationsClientId**
> UpdateApplications200Response patchApplicationsClientId()

Generate Client ID application

### Example

```typescript
import {
    ApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ApplicationApi(configuration);

let id: number; //application id (default to undefined)

const { status, data } = await apiInstance.patchApplicationsClientId(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | application id | defaults to undefined|


### Return type

**UpdateApplications200Response**

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

# **updateApplications**
> UpdateApplications200Response updateApplications(updateApplicationsRequest)

Update application

### Example

```typescript
import {
    ApplicationApi,
    Configuration,
    UpdateApplicationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ApplicationApi(configuration);

let id: number; //application id (default to undefined)
let updateApplicationsRequest: UpdateApplicationsRequest; //ActivityLog definition

const { status, data } = await apiInstance.updateApplications(
    id,
    updateApplicationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateApplicationsRequest** | **UpdateApplicationsRequest**| ActivityLog definition | |
| **id** | [**number**] | application id | defaults to undefined|


### Return type

**UpdateApplications200Response**

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

