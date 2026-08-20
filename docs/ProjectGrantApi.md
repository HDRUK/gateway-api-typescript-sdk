# ProjectGrantApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createProjectGrant**](#createprojectgrant) | **POST** /api/v1/project_grants | ProjectGrantController@store|
|[**fetchAllProjectGrants**](#fetchallprojectgrants) | **GET** /api/v1/project_grants | ProjectGrantController@index|
|[**fetchProjectGrant**](#fetchprojectgrant) | **GET** /api/v1/project_grants/{id} | ProjectGrantController@show|

# **createProjectGrant**
> CreateProjectGrant201Response createProjectGrant()

Create a project grant (and initial version)

### Example

```typescript
import {
    ProjectGrantApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectGrantApi(configuration);

const { status, data } = await apiInstance.createProjectGrant();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**CreateProjectGrant201Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Created |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchAllProjectGrants**
> FetchAllProjectGrants200Response fetchAllProjectGrants()

Get all project grants

### Example

```typescript
import {
    ProjectGrantApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectGrantApi(configuration);

let pid: string; //Filter by dataset pid (optional) (default to undefined)
let version: number; //Filter by dataset version number (optional) (default to undefined)
let projectGrantName: string; //Filter by project grant name (optional) (default to undefined)
let userId: number; //Filter by owning user id (optional) (default to undefined)
let teamId: number; //Filter by owning team id (optional) (default to undefined)
let withRelated: boolean; // (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllProjectGrants(
    pid,
    version,
    projectGrantName,
    userId,
    teamId,
    withRelated
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pid** | [**string**] | Filter by dataset pid | (optional) defaults to undefined|
| **version** | [**number**] | Filter by dataset version number | (optional) defaults to undefined|
| **projectGrantName** | [**string**] | Filter by project grant name | (optional) defaults to undefined|
| **userId** | [**number**] | Filter by owning user id | (optional) defaults to undefined|
| **teamId** | [**number**] | Filter by owning team id | (optional) defaults to undefined|
| **withRelated** | [**boolean**] |  | (optional) defaults to undefined|


### Return type

**FetchAllProjectGrants200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchProjectGrant**
> CountUniqueFieldsCollections200Response fetchProjectGrant()

Get a single project grant

### Example

```typescript
import {
    ProjectGrantApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectGrantApi(configuration);

let id: number; // (default to undefined)
let withRelated: boolean; // (optional) (default to undefined)

const { status, data } = await apiInstance.fetchProjectGrant(
    id,
    withRelated
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] |  | defaults to undefined|
| **withRelated** | [**boolean**] |  | (optional) defaults to undefined|


### Return type

**CountUniqueFieldsCollections200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

