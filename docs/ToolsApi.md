# ToolsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**countTeamUniqueFieldsToolsV2**](#countteamuniquefieldstoolsv2) | **GET** /api/v2/teams/{teamId}/tools/count/{field} | TeamToolController@count|
|[**countUniqueFieldsTools**](#countuniquefieldstools) | **GET** /api/v1/tools/count/{field} | ToolController@count|
|[**countUserUniqueFieldsToolsV2**](#countuseruniquefieldstoolsv2) | **GET** /api/v2/users/{userId}/tools/count/{field} | UserToolController@count|
|[**createTools**](#createtools) | **POST** /api/v1/tools | ToolController@store|
|[**createToolsByTeamV2**](#createtoolsbyteamv2) | **POST** /api/v2/teams/{teamId}/tools | ToolController@store|
|[**createToolsByUserV2**](#createtoolsbyuserv2) | **POST** /api/v2/users/{userId}/tools | UserToolController@store|
|[**createToolsIntegrations**](#createtoolsintegrations) | **POST** /api/v1/integrations/tools | IntegrationToolController@store|
|[**deleteTools**](#deletetools) | **DELETE** /api/v1/tools/{id} | ToolController@destroy|
|[**deleteToolsByTeamidV2**](#deletetoolsbyteamidv2) | **DELETE** /api/v2/teams/{teamId}/tools/{id} | TeamToolController@destroy|
|[**deleteToolsByUserV2**](#deletetoolsbyuserv2) | **DELETE** /api/v2/users/{userId}/tools/{id} | UserToolController@destroy|
|[**deleteToolsIntegrations**](#deletetoolsintegrations) | **DELETE** /api/v1/integrations/tools/{id} | IntegrationToolController@destroy|
|[**editTools**](#edittools) | **PATCH** /api/v1/tools/{id} | ToolController@edit|
|[**editToolsByTeamidV2**](#edittoolsbyteamidv2) | **PATCH** /api/v2/teams/{teamId}/tools/{id} | TeamToolController@edit|
|[**editToolsByUserV2**](#edittoolsbyuserv2) | **PATCH** /api/v2/users/{userId}/tools/{id} | UserToolController@edit|
|[**editToolsIntegrations**](#edittoolsintegrations) | **PATCH** /api/v1/integrations/tools/{id} | IntegrationToolController@edit|
|[**fetchAllToolByTeamAndStatusV2**](#fetchalltoolbyteamandstatusv2) | **GET** /api/v2/teams/{teamId}/tools/status/{status} | TeamToolController@indexStatus|
|[**fetchAllToolByUserAndStatusV2**](#fetchalltoolbyuserandstatusv2) | **GET** /api/v2/users/{userId}/tools/status/{status} | UserToolController@indexStatus|
|[**fetchAllTools**](#fetchalltools) | **GET** /api/v1/tools | Fetch all tools|
|[**fetchAllToolsIntegrations**](#fetchalltoolsintegrations) | **GET** /api/v1/integrations/tools | IntegrationToolController@index|
|[**fetchAllToolsV2**](#fetchalltoolsv2) | **GET** /api/v2/tools | ToolController@indexActive|
|[**fetchTools**](#fetchtools) | **GET** /api/v1/tools/{id} | ToolController@show|
|[**fetchToolsByTeamAndByIdV2**](#fetchtoolsbyteamandbyidv2) | **GET** /api/v2/teams/{teamId}/tools/{id} | TeamToolController@show|
|[**fetchToolsByUserAndByIdV2**](#fetchtoolsbyuserandbyidv2) | **GET** /api/v2/users/{userId}/tools/{id} | UserToolController@show|
|[**fetchToolsIntegrations**](#fetchtoolsintegrations) | **GET** /api/v1/integrations/tools/{id} | IntegrationToolController@show|
|[**fetchToolsV2**](#fetchtoolsv2) | **GET** /api/v2/tools/{id} | ToolController@showActive|
|[**updateTools**](#updatetools) | **PUT** /api/v1/tools/{id} | ToolController@update|
|[**updateToolsByTeamidV2**](#updatetoolsbyteamidv2) | **PUT** /api/v2/teams/{teamId}/tools/{id} | TeamToolController@update|
|[**updateToolsByUserV2**](#updatetoolsbyuserv2) | **PUT** /api/v2/users/{userId}/tools/{id} | UserToolController@update|
|[**updateToolsIntegrations**](#updatetoolsintegrations) | **PUT** /api/v1/integrations/tools/{id} | IntegrationToolController@update|

# **countTeamUniqueFieldsToolsV2**
> CountUniqueFieldsCollections200Response countTeamUniqueFieldsToolsV2()

Get team counts for distinct entries of a field in the model

### Example

```typescript
import {
    ToolsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let teamId: number; //team id (default to undefined)
let field: string; //name of the field to perform a count on (default to undefined)

const { status, data } = await apiInstance.countTeamUniqueFieldsToolsV2(
    teamId,
    field
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|
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

# **countUniqueFieldsTools**
> CountUniqueFieldsCollections200Response countUniqueFieldsTools()

Get Counts for distinct entries of a field in the model

### Example

```typescript
import {
    ToolsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let field: string; //name of the field to perform a count on (default to undefined)
let teamId: number; //team id (default to undefined)

const { status, data } = await apiInstance.countUniqueFieldsTools(
    field,
    teamId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **field** | [**string**] | name of the field to perform a count on | defaults to undefined|
| **teamId** | [**number**] | team id | defaults to undefined|


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

# **countUserUniqueFieldsToolsV2**
> CountUniqueFieldsCollections200Response countUserUniqueFieldsToolsV2()

Get user counts for distinct entries of a field in the model

### Example

```typescript
import {
    ToolsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let userId: number; //user id (default to undefined)
let field: string; //name of the field to perform a count on (default to undefined)

const { status, data } = await apiInstance.countUserUniqueFieldsToolsV2(
    userId,
    field
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | user id | defaults to undefined|
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

# **createTools**
> CreateCategories200Response createTools(createToolsRequest)

Create a new tool

### Example

```typescript
import {
    ToolsApi,
    Configuration,
    CreateToolsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let createToolsRequest: CreateToolsRequest; //Pass user credentials

const { status, data } = await apiInstance.createTools(
    createToolsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createToolsRequest** | **CreateToolsRequest**| Pass user credentials | |


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
|**400** | bad request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createToolsByTeamV2**
> CreateCategories200Response createToolsByTeamV2(createToolsRequest)

Create a new tool by team v2

### Example

```typescript
import {
    ToolsApi,
    Configuration,
    CreateToolsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let teamId: number; //team id (default to undefined)
let createToolsRequest: CreateToolsRequest; //Pass user credentials

const { status, data } = await apiInstance.createToolsByTeamV2(
    teamId,
    createToolsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createToolsRequest** | **CreateToolsRequest**| Pass user credentials | |
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
|**400** | bad request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createToolsByUserV2**
> CreateCategories200Response createToolsByUserV2(createToolsRequest)

Create a new tool by user v2

### Example

```typescript
import {
    ToolsApi,
    Configuration,
    CreateToolsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let userId: number; //user id (default to undefined)
let createToolsRequest: CreateToolsRequest; //Pass user credentials

const { status, data } = await apiInstance.createToolsByUserV2(
    userId,
    createToolsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createToolsRequest** | **CreateToolsRequest**| Pass user credentials | |
| **userId** | [**number**] | user id | defaults to undefined|


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
|**400** | bad request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createToolsIntegrations**
> CreateCategories200Response createToolsIntegrations(createToolsIntegrationsRequest)

Create a new tool

### Example

```typescript
import {
    ToolsApi,
    Configuration,
    CreateToolsIntegrationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let createToolsIntegrationsRequest: CreateToolsIntegrationsRequest; //Pass user credentials

const { status, data } = await apiInstance.createToolsIntegrations(
    createToolsIntegrationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createToolsIntegrationsRequest** | **CreateToolsIntegrationsRequest**| Pass user credentials | |


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
|**400** | bad request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteTools**
> DeleteFederation200Response deleteTools()

Delete tool by id

### Example

```typescript
import {
    ToolsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let id: number; //tool id (default to undefined)

const { status, data } = await apiInstance.deleteTools(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | tool id | defaults to undefined|


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

# **deleteToolsByTeamidV2**
> DeleteFederation200Response deleteToolsByTeamidV2()

Delete tool by id and by team_id

### Example

```typescript
import {
    ToolsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //tool id (default to undefined)

const { status, data } = await apiInstance.deleteToolsByTeamidV2(
    teamId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | tool id | defaults to undefined|


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

# **deleteToolsByUserV2**
> DeleteFederation200Response deleteToolsByUserV2()

Delete tool by id and by user

### Example

```typescript
import {
    ToolsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let userId: number; //user id (default to undefined)
let id: number; //tool id (default to undefined)

const { status, data } = await apiInstance.deleteToolsByUserV2(
    userId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | user id | defaults to undefined|
| **id** | [**number**] | tool id | defaults to undefined|


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

# **deleteToolsIntegrations**
> DeleteFederation200Response deleteToolsIntegrations()

Delete tool by id

### Example

```typescript
import {
    ToolsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let id: number; //tool id (default to undefined)

const { status, data } = await apiInstance.deleteToolsIntegrations(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | tool id | defaults to undefined|


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

# **editTools**
> FetchToolsIntegrations200Response editTools(updateToolsRequest)

Edit tool by id

### Example

```typescript
import {
    ToolsApi,
    Configuration,
    UpdateToolsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let id: number; //tool id (default to undefined)
let updateToolsRequest: UpdateToolsRequest; //Pass user credentials
let unarchive: string; //Unarchive a tool (optional) (default to undefined)

const { status, data } = await apiInstance.editTools(
    id,
    updateToolsRequest,
    unarchive
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateToolsRequest** | **UpdateToolsRequest**| Pass user credentials | |
| **id** | [**number**] | tool id | defaults to undefined|
| **unarchive** | [**string**] | Unarchive a tool | (optional) defaults to undefined|


### Return type

**FetchToolsIntegrations200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**400** | bad request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **editToolsByTeamidV2**
> FetchToolsIntegrations200Response editToolsByTeamidV2(updateToolsRequest)

Edit tool by id and by teamid

### Example

```typescript
import {
    ToolsApi,
    Configuration,
    UpdateToolsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //tool id (default to undefined)
let updateToolsRequest: UpdateToolsRequest; //Pass user credentials

const { status, data } = await apiInstance.editToolsByTeamidV2(
    teamId,
    id,
    updateToolsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateToolsRequest** | **UpdateToolsRequest**| Pass user credentials | |
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | tool id | defaults to undefined|


### Return type

**FetchToolsIntegrations200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**400** | bad request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **editToolsByUserV2**
> FetchToolsIntegrations200Response editToolsByUserV2(updateToolsRequest)

Edit tool by id and by user

### Example

```typescript
import {
    ToolsApi,
    Configuration,
    UpdateToolsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let userId: number; //user id (default to undefined)
let id: number; //tool id (default to undefined)
let updateToolsRequest: UpdateToolsRequest; //Pass user credentials

const { status, data } = await apiInstance.editToolsByUserV2(
    userId,
    id,
    updateToolsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateToolsRequest** | **UpdateToolsRequest**| Pass user credentials | |
| **userId** | [**number**] | user id | defaults to undefined|
| **id** | [**number**] | tool id | defaults to undefined|


### Return type

**FetchToolsIntegrations200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**400** | bad request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **editToolsIntegrations**
> FetchToolsIntegrations200Response editToolsIntegrations(updateToolsIntegrationsRequest)

Edit tool by id

### Example

```typescript
import {
    ToolsApi,
    Configuration,
    UpdateToolsIntegrationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let id: number; //tool id (default to undefined)
let updateToolsIntegrationsRequest: UpdateToolsIntegrationsRequest; //Pass user credentials

const { status, data } = await apiInstance.editToolsIntegrations(
    id,
    updateToolsIntegrationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateToolsIntegrationsRequest** | **UpdateToolsIntegrationsRequest**| Pass user credentials | |
| **id** | [**number**] | tool id | defaults to undefined|


### Return type

**FetchToolsIntegrations200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Created |  -  |
|**400** | bad request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchAllToolByTeamAndStatusV2**
> FetchAllToolsIntegrations200Response fetchAllToolByTeamAndStatusV2()

Returns a list of a teams tools with given status

### Example

```typescript
import {
    ToolsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let teamId: number; //ID of the team (default to undefined)
let status: 'active' | 'draft' | 'archived'; //Status of the tool (active, draft, or archived). Defaults to active if not provided. (default to 'active')

const { status, data } = await apiInstance.fetchAllToolByTeamAndStatusV2(
    teamId,
    status
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | ID of the team | defaults to undefined|
| **status** | [**&#39;active&#39; | &#39;draft&#39; | &#39;archived&#39;**]**Array<&#39;active&#39; &#124; &#39;draft&#39; &#124; &#39;archived&#39;>** | Status of the tool (active, draft, or archived). Defaults to active if not provided. | defaults to 'active'|


### Return type

**FetchAllToolsIntegrations200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchAllToolByUserAndStatusV2**
> FetchAllToolsIntegrations200Response fetchAllToolByUserAndStatusV2()

Returns a list of a user tools

### Example

```typescript
import {
    ToolsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let userId: number; //ID of the user (default to undefined)
let status: 'active' | 'draft' | 'archived'; //Status of the tool (active, draft, or archived). Defaults to active if not provided. (default to 'active')

const { status, data } = await apiInstance.fetchAllToolByUserAndStatusV2(
    userId,
    status
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | ID of the user | defaults to undefined|
| **status** | [**&#39;active&#39; | &#39;draft&#39; | &#39;archived&#39;**]**Array<&#39;active&#39; &#124; &#39;draft&#39; &#124; &#39;archived&#39;>** | Status of the tool (active, draft, or archived). Defaults to active if not provided. | defaults to 'active'|


### Return type

**FetchAllToolsIntegrations200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchAllTools**
> FetchAllTools200Response fetchAllTools()

Get all tools with optional filters and sorting

### Example

```typescript
import {
    ToolsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let mongoId: string; //Filter tools by mongo ID (optional) (default to undefined)
let teamId: number; //Filter tools by team ID (optional) (default to undefined)
let userId: number; //Filter tools by user ID (optional) (default to undefined)
let title: string; //Filter tools by title (optional) (default to undefined)
let sort: string; //Sort tools by a specific field and direction, e.g., \'name:asc\' or \'created_at:desc\' (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllTools(
    mongoId,
    teamId,
    userId,
    title,
    sort
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **mongoId** | [**string**] | Filter tools by mongo ID | (optional) defaults to undefined|
| **teamId** | [**number**] | Filter tools by team ID | (optional) defaults to undefined|
| **userId** | [**number**] | Filter tools by user ID | (optional) defaults to undefined|
| **title** | [**string**] | Filter tools by title | (optional) defaults to undefined|
| **sort** | [**string**] | Sort tools by a specific field and direction, e.g., \&#39;name:asc\&#39; or \&#39;created_at:desc\&#39; | (optional) defaults to undefined|


### Return type

**FetchAllTools200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**400** | Bad request response |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchAllToolsIntegrations**
> FetchAllToolsIntegrations200Response fetchAllToolsIntegrations()

Get All Tools

### Example

```typescript
import {
    ToolsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

const { status, data } = await apiInstance.fetchAllToolsIntegrations();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**FetchAllToolsIntegrations200Response**

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

# **fetchAllToolsV2**
> FetchAllTools200Response fetchAllToolsV2()

Get all tools with optional filters and sorting

### Example

```typescript
import {
    ToolsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let name: string; //Filter tools by name (optional) (default to undefined)
let sort: string; //Sort tools by a specific field and direction, e.g., \'name:asc\' or \'created_at:desc\' (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllToolsV2(
    name,
    sort
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **name** | [**string**] | Filter tools by name | (optional) defaults to undefined|
| **sort** | [**string**] | Sort tools by a specific field and direction, e.g., \&#39;name:asc\&#39; or \&#39;created_at:desc\&#39; | (optional) defaults to undefined|


### Return type

**FetchAllTools200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**400** | Bad request response |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchTools**
> FetchToolsIntegrations200Response fetchTools()

Get tool by id

### Example

```typescript
import {
    ToolsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let id: number; //tool id (default to undefined)
let viewType: string; //Query flag to show full tool data or a trimmed version (defaults to full). (optional) (default to 'full')

const { status, data } = await apiInstance.fetchTools(
    id,
    viewType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | tool id | defaults to undefined|
| **viewType** | [**string**] | Query flag to show full tool data or a trimmed version (defaults to full). | (optional) defaults to 'full'|


### Return type

**FetchToolsIntegrations200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**401** | Unauthorized |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchToolsByTeamAndByIdV2**
> FetchToolsIntegrations200Response fetchToolsByTeamAndByIdV2()

Get tool by team id and by id

### Example

```typescript
import {
    ToolsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //tool id (default to undefined)
let viewType: string; //Query flag to show full tool data or a trimmed version (defaults to full). (optional) (default to 'full')

const { status, data } = await apiInstance.fetchToolsByTeamAndByIdV2(
    teamId,
    id,
    viewType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | tool id | defaults to undefined|
| **viewType** | [**string**] | Query flag to show full tool data or a trimmed version (defaults to full). | (optional) defaults to 'full'|


### Return type

**FetchToolsIntegrations200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**401** | Unauthorized |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchToolsByUserAndByIdV2**
> FetchToolsIntegrations200Response fetchToolsByUserAndByIdV2()

Get tool by user id and by id

### Example

```typescript
import {
    ToolsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let userId: number; //user id (default to undefined)
let id: number; //tool id (default to undefined)
let viewType: string; //Query flag to show full tool data or a trimmed version (defaults to full). (optional) (default to 'full')

const { status, data } = await apiInstance.fetchToolsByUserAndByIdV2(
    userId,
    id,
    viewType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | user id | defaults to undefined|
| **id** | [**number**] | tool id | defaults to undefined|
| **viewType** | [**string**] | Query flag to show full tool data or a trimmed version (defaults to full). | (optional) defaults to 'full'|


### Return type

**FetchToolsIntegrations200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**401** | Unauthorized |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchToolsIntegrations**
> FetchToolsIntegrations200Response fetchToolsIntegrations()

Get tool by id

### Example

```typescript
import {
    ToolsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let id: number; //tool id (default to undefined)

const { status, data } = await apiInstance.fetchToolsIntegrations(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | tool id | defaults to undefined|


### Return type

**FetchToolsIntegrations200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**401** | Unauthorized |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchToolsV2**
> FetchToolsIntegrations200Response fetchToolsV2()

Get tool by id

### Example

```typescript
import {
    ToolsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let id: number; //tool id (default to undefined)

const { status, data } = await apiInstance.fetchToolsV2(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | tool id | defaults to undefined|


### Return type

**FetchToolsIntegrations200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**401** | Unauthorized |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateTools**
> FetchToolsIntegrations200Response updateTools(updateToolsRequest)

Update tool by id

### Example

```typescript
import {
    ToolsApi,
    Configuration,
    UpdateToolsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let id: number; //tool id (default to undefined)
let updateToolsRequest: UpdateToolsRequest; //Pass user credentials

const { status, data } = await apiInstance.updateTools(
    id,
    updateToolsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateToolsRequest** | **UpdateToolsRequest**| Pass user credentials | |
| **id** | [**number**] | tool id | defaults to undefined|


### Return type

**FetchToolsIntegrations200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**400** | bad request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateToolsByTeamidV2**
> FetchToolsIntegrations200Response updateToolsByTeamidV2(updateToolsRequest)

Update tools by team id

### Example

```typescript
import {
    ToolsApi,
    Configuration,
    UpdateToolsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //tool id (default to undefined)
let updateToolsRequest: UpdateToolsRequest; //Pass user credentials

const { status, data } = await apiInstance.updateToolsByTeamidV2(
    teamId,
    id,
    updateToolsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateToolsRequest** | **UpdateToolsRequest**| Pass user credentials | |
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | tool id | defaults to undefined|


### Return type

**FetchToolsIntegrations200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**400** | bad request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateToolsByUserV2**
> FetchToolsIntegrations200Response updateToolsByUserV2(updateToolsRequest)

Update tools by user id

### Example

```typescript
import {
    ToolsApi,
    Configuration,
    UpdateToolsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let userId: number; //user id (default to undefined)
let id: number; //tool id (default to undefined)
let updateToolsRequest: UpdateToolsRequest; //Pass user credentials

const { status, data } = await apiInstance.updateToolsByUserV2(
    userId,
    id,
    updateToolsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateToolsRequest** | **UpdateToolsRequest**| Pass user credentials | |
| **userId** | [**number**] | user id | defaults to undefined|
| **id** | [**number**] | tool id | defaults to undefined|


### Return type

**FetchToolsIntegrations200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**400** | bad request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateToolsIntegrations**
> FetchToolsIntegrations200Response updateToolsIntegrations(updateToolsIntegrationsRequest)

Update tool by id

### Example

```typescript
import {
    ToolsApi,
    Configuration,
    UpdateToolsIntegrationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ToolsApi(configuration);

let id: number; //tool id (default to undefined)
let updateToolsIntegrationsRequest: UpdateToolsIntegrationsRequest; //Pass user credentials

const { status, data } = await apiInstance.updateToolsIntegrations(
    id,
    updateToolsIntegrationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateToolsIntegrationsRequest** | **UpdateToolsIntegrationsRequest**| Pass user credentials | |
| **id** | [**number**] | tool id | defaults to undefined|


### Return type

**FetchToolsIntegrations200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Created |  -  |
|**400** | bad request |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

