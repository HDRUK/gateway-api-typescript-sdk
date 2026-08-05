# TeamDataAccessApplicationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**countTeamDarApplications**](#countteamdarapplications) | **GET** /api/v1/teams/{teamId}/dar/applications/count | TeamDataAccessApplicationController@allCounts|
|[**countUniqueFieldsDarApplications**](#countuniquefieldsdarapplications) | **GET** /api/v1/teams/{teamId}/dar/applications/count/{field} | TeamDataAccessApplicationController@count|
|[**fetchTeamDarApplication**](#fetchteamdarapplication) | **GET** /api/v1/teams/{teamId}/dar/applications/{id} | TeamDataAccessApplicationController@show|
|[**fetchTeamDarApplications**](#fetchteamdarapplications) | **GET** /api/v1/teams/{teamId}/dar/applications | TeamDataAccessApplicationController@index|

# **countTeamDarApplications**
> CountUniqueFieldsCollections200Response countTeamDarApplications()

Get Counts for all status fields in the model

### Example

```typescript
import {
    TeamDataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDataAccessApplicationApi(configuration);

let teamId: number; //Team id (default to undefined)

const { status, data } = await apiInstance.countTeamDarApplications(
    teamId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team id | defaults to undefined|


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

# **countUniqueFieldsDarApplications**
> CountUniqueFieldsCollections200Response countUniqueFieldsDarApplications()

Get Counts for distinct entries of a field in the model

### Example

```typescript
import {
    TeamDataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDataAccessApplicationApi(configuration);

let teamId: number; //Team id (default to undefined)
let field: string; //name of the field to perform a count on (default to undefined)

const { status, data } = await apiInstance.countUniqueFieldsDarApplications(
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

# **fetchTeamDarApplication**
> FetchTeamDarApplication200Response fetchTeamDarApplication()

Return a single DAR application

### Example

```typescript
import {
    TeamDataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDataAccessApplicationApi(configuration);

let teamId: number; //Team id (default to undefined)
let id: number; //DAR application id (default to undefined)

const { status, data } = await apiInstance.fetchTeamDarApplication(
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

**FetchTeamDarApplication200Response**

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

# **fetchTeamDarApplications**
> FetchTeamDarApplications200Response fetchTeamDarApplications()

List of dar applications belonging to a team

### Example

```typescript
import {
    TeamDataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDataAccessApplicationApi(configuration);

let teamId: number; //Team id (default to undefined)

const { status, data } = await apiInstance.fetchTeamDarApplications(
    teamId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team id | defaults to undefined|


### Return type

**FetchTeamDarApplications200Response**

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

