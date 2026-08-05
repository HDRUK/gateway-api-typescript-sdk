# TeamDataAccessTemplateApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**deleteTeamDarTemplateFile**](#deleteteamdartemplatefile) | **DELETE** /api/v1/teams/{teamId}/dar/templates/{id}/files/{fileId} | TeamDataAccessTemplateController@destroyFile|
|[**fetchTeamDarTemplates**](#fetchteamdartemplates) | **GET** /api/v1/teams/{teamId}/dar/templates | TeamDataAccessTemplateController@index|
|[**teamDarTemplateCountUniqueFields**](#teamdartemplatecountuniquefields) | **GET** /api/v1/teams/{teamId}/dar/templates/count/{field} | TeamDataAccessTemplateController@count|

# **deleteTeamDarTemplateFile**
> DeleteApplications200Response deleteTeamDarTemplateFile()

Delete a file associated with a DAR template

### Example

```typescript
import {
    TeamDataAccessTemplateApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDataAccessTemplateApi(configuration);

let teamId: number; //Team id (default to undefined)
let id: number; //DAR template id (default to undefined)
let fileId: string; //File id (default to undefined)

const { status, data } = await apiInstance.deleteTeamDarTemplateFile(
    teamId,
    id,
    fileId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team id | defaults to undefined|
| **id** | [**number**] | DAR template id | defaults to undefined|
| **fileId** | [**string**] | File id | defaults to undefined|


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
|**401** | Unauthorized |  -  |
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchTeamDarTemplates**
> FetchDarTemplates200Response fetchTeamDarTemplates()

List of dar templates belonging to a team

### Example

```typescript
import {
    TeamDataAccessTemplateApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDataAccessTemplateApi(configuration);

let teamId: number; //Team id (default to undefined)
let published: string; //Template publication status to filter by (true, false) (optional) (default to undefined)

const { status, data } = await apiInstance.fetchTeamDarTemplates(
    teamId,
    published
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team id | defaults to undefined|
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

# **teamDarTemplateCountUniqueFields**
> CountUniqueFieldsCollections200Response teamDarTemplateCountUniqueFields()

Get Counts for distinct entries of a field in the model

### Example

```typescript
import {
    TeamDataAccessTemplateApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDataAccessTemplateApi(configuration);

let teamId: number; //Team id (default to undefined)
let field: string; //name of the field to perform a count on (default to undefined)

const { status, data } = await apiInstance.teamDarTemplateCountUniqueFields(
    teamId,
    field
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team id | defaults to undefined|
| **field** | [**string**] | name of the field to perform a count on | defaults to undefined|


### Return type

**CountUniqueFieldsCollections200Response**

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

