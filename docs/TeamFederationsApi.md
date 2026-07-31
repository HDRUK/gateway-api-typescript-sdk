# TeamFederationsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createFederationTeam**](#createfederationteam) | **POST** /api/v1/teams/{teamId}/federations | FederationController@store|
|[**deleteFederation**](#deletefederation) | **DELETE** /api/v1/teams/{teamId}/federations/{federationId} | FederationController@destroy|
|[**editFederationTeam**](#editfederationteam) | **PATCH** /api/v1/teams/{teamId}/federations/{federationId} | FederationController@edit|
|[**getFederationByFederationIdAndTeamId**](#getfederationbyfederationidandteamid) | **GET** /api/v1/teams/{teamId}/federations/{federationId} | FederationController@show|
|[**getFederationHistory**](#getfederationhistory) | **GET** /api/v1/teams/{teamId}/federations/{federationId}/history | FederationController@history|
|[**getFederationTeamId**](#getfederationteamid) | **GET** /api/v1/teams/{teamId}/federations | FederationController@index|
|[**runFederation**](#runfederation) | **GET** /api/v1/teams/{teamId}/federations/{federationId}/run | FederationController@runNow|
|[**testFederation**](#testfederation) | **POST** /api/v1/teams/{teamId}/federations/test | FederationController@testFederation|
|[**updateFederationTeam**](#updatefederationteam) | **PUT** /api/v1/teams/{teamId}/federations/{federationId} | FederationController@update|

# **createFederationTeam**
> CreateCategories200Response createFederationTeam(createFederationTeamRequest)

Create federation

### Example

```typescript
import {
    TeamFederationsApi,
    Configuration,
    CreateFederationTeamRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamFederationsApi(configuration);

let teamId: number; //team id (default to undefined)
let createFederationTeamRequest: CreateFederationTeamRequest; //Pass user credentials

const { status, data } = await apiInstance.createFederationTeam(
    teamId,
    createFederationTeamRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createFederationTeamRequest** | **CreateFederationTeamRequest**| Pass user credentials | |
| **teamId** | [**number**] | team id | defaults to undefined|


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
|**201** | Created |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteFederation**
> DeleteFederation200Response deleteFederation()

Delete federation for team

### Example

```typescript
import {
    TeamFederationsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamFederationsApi(configuration);

let teamId: number; //team id (default to undefined)
let federationId: number; //federation id (default to undefined)

const { status, data } = await apiInstance.deleteFederation(
    teamId,
    federationId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|
| **federationId** | [**number**] | federation id | defaults to undefined|


### Return type

**DeleteFederation200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**404** | Error response |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **editFederationTeam**
> CreateCategories200Response editFederationTeam(createFederationTeamRequest)

Edit federation for team

### Example

```typescript
import {
    TeamFederationsApi,
    Configuration,
    CreateFederationTeamRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamFederationsApi(configuration);

let teamId: number; //team id (default to undefined)
let federationId: number; //federation id (default to undefined)
let createFederationTeamRequest: CreateFederationTeamRequest; //Pass user credentials

const { status, data } = await apiInstance.editFederationTeam(
    teamId,
    federationId,
    createFederationTeamRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createFederationTeamRequest** | **CreateFederationTeamRequest**| Pass user credentials | |
| **teamId** | [**number**] | team id | defaults to undefined|
| **federationId** | [**number**] | federation id | defaults to undefined|


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
|**201** | Created |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getFederationByFederationIdAndTeamId**
> GetFederationByFederationIdAndTeamId200Response getFederationByFederationIdAndTeamId()

Get federation by federation id from team id

### Example

```typescript
import {
    TeamFederationsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamFederationsApi(configuration);

let teamId: number; //team id (default to undefined)
let federationId: number; //federation id (default to undefined)

const { status, data } = await apiInstance.getFederationByFederationIdAndTeamId(
    teamId,
    federationId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|
| **federationId** | [**number**] | federation id | defaults to undefined|


### Return type

**GetFederationByFederationIdAndTeamId200Response**

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

# **getFederationHistory**
> GetFederationHistory200Response getFederationHistory()

Get run history for a federation

### Example

```typescript
import {
    TeamFederationsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamFederationsApi(configuration);

let teamId: number; //team id (default to undefined)
let federationId: number; //federation id (default to undefined)
let perPage: number; //per page (optional) (default to undefined)

const { status, data } = await apiInstance.getFederationHistory(
    teamId,
    federationId,
    perPage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|
| **federationId** | [**number**] | federation id | defaults to undefined|
| **perPage** | [**number**] | per page | (optional) defaults to undefined|


### Return type

**GetFederationHistory200Response**

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

# **getFederationTeamId**
> GetFederationTeamId200Response getFederationTeamId()

Get federations by team id

### Example

```typescript
import {
    TeamFederationsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamFederationsApi(configuration);

let teamId: number; //team id (default to undefined)

const { status, data } = await apiInstance.getFederationTeamId(
    teamId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|


### Return type

**GetFederationTeamId200Response**

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

# **runFederation**
> TestFederation200Response runFederation()

Run federation immediately

### Example

```typescript
import {
    TeamFederationsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamFederationsApi(configuration);

let teamId: number; //team id (default to undefined)
let federationId: number; //federation id (default to undefined)

const { status, data } = await apiInstance.runFederation(
    teamId,
    federationId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|
| **federationId** | [**number**] | federation id | defaults to undefined|


### Return type

**TestFederation200Response**

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

# **testFederation**
> TestFederation200Response testFederation()

Test federation configuration

### Example

```typescript
import {
    TeamFederationsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamFederationsApi(configuration);

let teamId: number; //team id (default to undefined)

const { status, data } = await apiInstance.testFederation(
    teamId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|


### Return type

**TestFederation200Response**

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

# **updateFederationTeam**
> CreateCategories200Response updateFederationTeam(updateFederationTeamRequest)

Update federation for team

### Example

```typescript
import {
    TeamFederationsApi,
    Configuration,
    UpdateFederationTeamRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamFederationsApi(configuration);

let teamId: number; //team id (default to undefined)
let federationId: number; //federation id (default to undefined)
let updateFederationTeamRequest: UpdateFederationTeamRequest; //Pass user credentials

const { status, data } = await apiInstance.updateFederationTeam(
    teamId,
    federationId,
    updateFederationTeamRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateFederationTeamRequest** | **UpdateFederationTeamRequest**| Pass user credentials | |
| **teamId** | [**number**] | team id | defaults to undefined|
| **federationId** | [**number**] | federation id | defaults to undefined|


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
|**201** | Created |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

