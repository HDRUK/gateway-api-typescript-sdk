# PublicationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**countTeamUniqueFieldsPublicationV2**](#countteamuniquefieldspublicationv2) | **GET** /api/v2/teams/{teamId}/publications/count/{field} | TeamPublicationController@count|
|[**countUniqueFieldsPublications**](#countuniquefieldspublications) | **GET** /api/v1/publication/count/{field} | PublicationController@count|
|[**countUserUniqueFieldsPublicationV2**](#countuseruniquefieldspublicationv2) | **GET** /api/v2/users/{userId}/publications/count/{field} | UserPublicationController@count|
|[**createPublications**](#createpublications) | **POST** /api/v1/publications | PublicationController@store|
|[**createPublicationsV2ByTeamId**](#createpublicationsv2byteamid) | **POST** /api/v2/teams/{teamId}/publications | TeamPublicationController@store|
|[**createPublicationsV2ByUserId**](#createpublicationsv2byuserid) | **POST** /api/v2/users/{userId}/publications | UserPublicationController@store|
|[**deletePublications**](#deletepublications) | **DELETE** /api/v1/publications/{id} | PublicationController@destroy|
|[**deletePublicationsV2ByTeamId**](#deletepublicationsv2byteamid) | **DELETE** /api/v2/teams/{teamId}/publications/{id} | TeamPublicationController@destroy|
|[**deletePublicationsV2ByUserId**](#deletepublicationsv2byuserid) | **DELETE** /api/v2/users/{userId}/publications/{id} | UserPublicationController@destroy|
|[**editPublications**](#editpublications) | **PATCH** /api/v1/publications/{id} | PublicationController@edit|
|[**editPublicationsV2ByTeamId**](#editpublicationsv2byteamid) | **PATCH** /api/v2/teams/{teamId}/publications/{id} | TeamPublicationController@edit|
|[**editPublicationsV2ByUserId**](#editpublicationsv2byuserid) | **PATCH** /api/v2/users/{userId}/publications/{id} | UserPublicationController@edit|
|[**fetchAllPublications**](#fetchallpublications) | **GET** /api/v1/publications | PublicationController@index|
|[**fetchAllPublicationsByTeamAndStatusV2**](#fetchallpublicationsbyteamandstatusv2) | **GET** /api/v2/teams/{teamId}/publications/status/{status} | TeamPublicationController@indexStatus|
|[**fetchAllPublicationsByUserAndStatusV2**](#fetchallpublicationsbyuserandstatusv2) | **GET** /api/v2/users/{userId}/publications/{status} | UserPublicationController@indexStatus|
|[**fetchAllPublicationsV2**](#fetchallpublicationsv2) | **GET** /api/v2/publications | PublicationController@indexActive|
|[**fetchPublications**](#fetchpublications) | **GET** /api/v1/publications/{id} | PublicationController@show|
|[**fetchPublicationsByTeamAndByIdV2**](#fetchpublicationsbyteamandbyidv2) | **GET** /api/v2/teams/{teamId}/publications/{id} | TeamPublicationController@show|
|[**fetchPublicationsByUserAndByIdV2**](#fetchpublicationsbyuserandbyidv2) | **GET** /api/v2/users/{userId}/publications/{id} | UserPublicationController@show|
|[**fetchPublicationsV2**](#fetchpublicationsv2) | **GET** /api/v2/publications/{id} | PublicationController@showActive|
|[**updatePublications**](#updatepublications) | **PUT** /api/v1/publications/{id} | PublicationController@update|
|[**updatePublicationsV2ByTeamId**](#updatepublicationsv2byteamid) | **PUT** /api/v2/teams/{teamId}/publications/{id} | TeamPublicationController@update|
|[**updatePublicationsV2ByUserId**](#updatepublicationsv2byuserid) | **PUT** /api/v2/users/{userId}/publications/{id} | UserPublicationController@update|

# **countTeamUniqueFieldsPublicationV2**
> CountUniqueFieldsCollections200Response countTeamUniqueFieldsPublicationV2()

Get team counts for distinct entries of a field in the model

### Example

```typescript
import {
    PublicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let teamId: number; //team id (default to undefined)
let field: string; //name of the field to perform a count on (default to undefined)

const { status, data } = await apiInstance.countTeamUniqueFieldsPublicationV2(
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

# **countUniqueFieldsPublications**
> CountUniqueFieldsCollections200Response countUniqueFieldsPublications()

Get Counts for distinct entries of a field in the model

### Example

```typescript
import {
    PublicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let field: string; //name of the field to perform a count on (default to undefined)
let ownerId: number; //owner id (default to undefined)
let teamId: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.countUniqueFieldsPublications(
    field,
    ownerId,
    teamId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **field** | [**string**] | name of the field to perform a count on | defaults to undefined|
| **ownerId** | [**number**] | owner id | defaults to undefined|
| **teamId** | [**number**] |  | (optional) defaults to undefined|


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

# **countUserUniqueFieldsPublicationV2**
> CountUniqueFieldsCollections200Response countUserUniqueFieldsPublicationV2()

Get user counts for distinct entries of a field in the model

### Example

```typescript
import {
    PublicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let userId: number; //user id (default to undefined)
let field: string; //name of the field to perform a count on (default to undefined)

const { status, data } = await apiInstance.countUserUniqueFieldsPublicationV2(
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

# **createPublications**
> CreateCategories200Response createPublications(createPublicationsRequest)

Create a new publication

### Example

```typescript
import {
    PublicationApi,
    Configuration,
    CreatePublicationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let createPublicationsRequest: CreatePublicationsRequest; //Pass user credentials

const { status, data } = await apiInstance.createPublications(
    createPublicationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createPublicationsRequest** | **CreatePublicationsRequest**| Pass user credentials | |


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

# **createPublicationsV2ByTeamId**
> CreateCategories200Response createPublicationsV2ByTeamId(createPublicationsRequest)

Create a new publication by team id

### Example

```typescript
import {
    PublicationApi,
    Configuration,
    CreatePublicationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let teamId: number; //team id (default to undefined)
let createPublicationsRequest: CreatePublicationsRequest; //Pass user credentials

const { status, data } = await apiInstance.createPublicationsV2ByTeamId(
    teamId,
    createPublicationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createPublicationsRequest** | **CreatePublicationsRequest**| Pass user credentials | |
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

# **createPublicationsV2ByUserId**
> CreateCategories200Response createPublicationsV2ByUserId(createPublicationsRequest)

Create a new publication by user id

### Example

```typescript
import {
    PublicationApi,
    Configuration,
    CreatePublicationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let userId: number; //ID of the user (default to undefined)
let createPublicationsRequest: CreatePublicationsRequest; //Pass user credentials

const { status, data } = await apiInstance.createPublicationsV2ByUserId(
    userId,
    createPublicationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createPublicationsRequest** | **CreatePublicationsRequest**| Pass user credentials | |
| **userId** | [**number**] | ID of the user | defaults to undefined|


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

# **deletePublications**
> DeleteFederation200Response deletePublications()

Delete publication by id

### Example

```typescript
import {
    PublicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let id: number; //publication id (default to undefined)

const { status, data } = await apiInstance.deletePublications(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | publication id | defaults to undefined|


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
|**401** | Unauthorized |  -  |
|**404** | Error response |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deletePublicationsV2ByTeamId**
> DeleteFederation200Response deletePublicationsV2ByTeamId()

Delete publication by team id and id

### Example

```typescript
import {
    PublicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //publication id (default to undefined)

const { status, data } = await apiInstance.deletePublicationsV2ByTeamId(
    teamId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | publication id | defaults to undefined|


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
|**401** | Unauthorized |  -  |
|**404** | Error response |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deletePublicationsV2ByUserId**
> DeleteFederation200Response deletePublicationsV2ByUserId()

Delete publication by user id and id

### Example

```typescript
import {
    PublicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let userId: number; //ID of the user (default to undefined)
let id: number; //publication id (default to undefined)

const { status, data } = await apiInstance.deletePublicationsV2ByUserId(
    userId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | ID of the user | defaults to undefined|
| **id** | [**number**] | publication id | defaults to undefined|


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
|**401** | Unauthorized |  -  |
|**404** | Error response |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **editPublications**
> FetchPublications200Response editPublications(updatePublicationsRequest)

Edit publications

### Example

```typescript
import {
    PublicationApi,
    Configuration,
    UpdatePublicationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let id: number; //publications id (default to undefined)
let updatePublicationsRequest: UpdatePublicationsRequest; //Pass user credentials
let unarchive: string; //Unarchive a publication (optional) (default to undefined)

const { status, data } = await apiInstance.editPublications(
    id,
    updatePublicationsRequest,
    unarchive
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updatePublicationsRequest** | **UpdatePublicationsRequest**| Pass user credentials | |
| **id** | [**number**] | publications id | defaults to undefined|
| **unarchive** | [**string**] | Unarchive a publication | (optional) defaults to undefined|


### Return type

**FetchPublications200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**400** | Error |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **editPublicationsV2ByTeamId**
> FetchPublications200Response editPublicationsV2ByTeamId(updatePublicationsRequest)

Edit publications by team id

### Example

```typescript
import {
    PublicationApi,
    Configuration,
    UpdatePublicationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //publications id (default to undefined)
let updatePublicationsRequest: UpdatePublicationsRequest; //Pass user credentials

const { status, data } = await apiInstance.editPublicationsV2ByTeamId(
    teamId,
    id,
    updatePublicationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updatePublicationsRequest** | **UpdatePublicationsRequest**| Pass user credentials | |
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | publications id | defaults to undefined|


### Return type

**FetchPublications200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**400** | Error |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **editPublicationsV2ByUserId**
> FetchPublications200Response editPublicationsV2ByUserId(updatePublicationsRequest)

Edit publications by user id

### Example

```typescript
import {
    PublicationApi,
    Configuration,
    UpdatePublicationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let userId: number; //ID of the user (default to undefined)
let id: number; //publications id (default to undefined)
let updatePublicationsRequest: UpdatePublicationsRequest; //Pass user credentials

const { status, data } = await apiInstance.editPublicationsV2ByUserId(
    userId,
    id,
    updatePublicationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updatePublicationsRequest** | **UpdatePublicationsRequest**| Pass user credentials | |
| **userId** | [**number**] | ID of the user | defaults to undefined|
| **id** | [**number**] | publications id | defaults to undefined|


### Return type

**FetchPublications200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**400** | Error |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchAllPublications**
> FetchAllPublications200Response fetchAllPublications()

Get All Publications

### Example

```typescript
import {
    PublicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let paperTitle: string; //Filter tools by paper title (optional) (default to undefined)
let ownerId: number; //Filter tools by owner id (optional) (default to undefined)
let teamId: number; //Filter tools by team id (optional) (default to undefined)
let status: string; //Publication status to filter by (\'ACTIVE\', \'DRAFT\', \'ARCHIVED\') (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllPublications(
    paperTitle,
    ownerId,
    teamId,
    status
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **paperTitle** | [**string**] | Filter tools by paper title | (optional) defaults to undefined|
| **ownerId** | **number** | Filter tools by owner id | (optional) defaults to undefined|
| **teamId** | **number** | Filter tools by team id | (optional) defaults to undefined|
| **status** | [**string**] | Publication status to filter by (\&#39;ACTIVE\&#39;, \&#39;DRAFT\&#39;, \&#39;ARCHIVED\&#39;) | (optional) defaults to undefined|


### Return type

**FetchAllPublications200Response**

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

# **fetchAllPublicationsByTeamAndStatusV2**
> FetchAllPublications200Response fetchAllPublicationsByTeamAndStatusV2()

Returns a list of a teams publications

### Example

```typescript
import {
    PublicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let teamId: number; //ID of the team (default to undefined)
let status: 'active' | 'draft' | 'archived'; //Status of the team (active, draft, or archived). Defaults to active if not provided. (default to 'active')
let paperTitle: string; //Filter Publication by title (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllPublicationsByTeamAndStatusV2(
    teamId,
    status,
    paperTitle
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | ID of the team | defaults to undefined|
| **status** | [**&#39;active&#39; | &#39;draft&#39; | &#39;archived&#39;**]**Array<&#39;active&#39; &#124; &#39;draft&#39; &#124; &#39;archived&#39;>** | Status of the team (active, draft, or archived). Defaults to active if not provided. | defaults to 'active'|
| **paperTitle** | [**string**] | Filter Publication by title | (optional) defaults to undefined|


### Return type

**FetchAllPublications200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchAllPublicationsByUserAndStatusV2**
> FetchAllPublications200Response fetchAllPublicationsByUserAndStatusV2()

Returns a list of a users publications

### Example

```typescript
import {
    PublicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let userId: number; //ID of the user (default to undefined)
let status: 'active' | 'draft' | 'archived'; //Status of the team (active, draft, or archived). Defaults to active if not provided. (default to 'active')
let paperTitle: string; //Filter Publication by title (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllPublicationsByUserAndStatusV2(
    userId,
    status,
    paperTitle
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | ID of the user | defaults to undefined|
| **status** | [**&#39;active&#39; | &#39;draft&#39; | &#39;archived&#39;**]**Array<&#39;active&#39; &#124; &#39;draft&#39; &#124; &#39;archived&#39;>** | Status of the team (active, draft, or archived). Defaults to active if not provided. | defaults to 'active'|
| **paperTitle** | [**string**] | Filter Publication by title | (optional) defaults to undefined|


### Return type

**FetchAllPublications200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchAllPublicationsV2**
> FetchAllPublications200Response fetchAllPublicationsV2()

Get All Publications

### Example

```typescript
import {
    PublicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let paperTitle: string; //Filter tools by paper title (optional) (default to undefined)
let withRelated: boolean; //Return related datasets (optional) (default to undefined)
let perPage: number; //per page (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllPublicationsV2(
    paperTitle,
    withRelated,
    perPage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **paperTitle** | [**string**] | Filter tools by paper title | (optional) defaults to undefined|
| **withRelated** | [**boolean**] | Return related datasets | (optional) defaults to undefined|
| **perPage** | [**number**] | per page | (optional) defaults to undefined|


### Return type

**FetchAllPublications200Response**

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

# **fetchPublications**
> FetchPublications200Response fetchPublications()

Get publication by id

### Example

```typescript
import {
    PublicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let id: number; //publication id (default to undefined)

const { status, data } = await apiInstance.fetchPublications(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | publication id | defaults to undefined|


### Return type

**FetchPublications200Response**

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

# **fetchPublicationsByTeamAndByIdV2**
> FetchPublications200Response fetchPublicationsByTeamAndByIdV2()

Get publication by team id and by id

### Example

```typescript
import {
    PublicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //publication id (default to undefined)

const { status, data } = await apiInstance.fetchPublicationsByTeamAndByIdV2(
    teamId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | publication id | defaults to undefined|


### Return type

**FetchPublications200Response**

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

# **fetchPublicationsByUserAndByIdV2**
> FetchPublications200Response fetchPublicationsByUserAndByIdV2()

Get publication by user id and by id

### Example

```typescript
import {
    PublicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let userId: number; //ID of the user (default to undefined)
let id: number; //publication id (default to undefined)

const { status, data } = await apiInstance.fetchPublicationsByUserAndByIdV2(
    userId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | ID of the user | defaults to undefined|
| **id** | [**number**] | publication id | defaults to undefined|


### Return type

**FetchPublications200Response**

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

# **fetchPublicationsV2**
> FetchPublications200Response fetchPublicationsV2()

Get publication by id

### Example

```typescript
import {
    PublicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let id: number; //publication id (default to undefined)

const { status, data } = await apiInstance.fetchPublicationsV2(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | publication id | defaults to undefined|


### Return type

**FetchPublications200Response**

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

# **updatePublications**
> FetchPublications200Response updatePublications(updatePublicationsRequest)

Update publications

### Example

```typescript
import {
    PublicationApi,
    Configuration,
    UpdatePublicationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let id: number; //publication id (default to undefined)
let updatePublicationsRequest: UpdatePublicationsRequest; //Pass user credentials

const { status, data } = await apiInstance.updatePublications(
    id,
    updatePublicationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updatePublicationsRequest** | **UpdatePublicationsRequest**| Pass user credentials | |
| **id** | [**number**] | publication id | defaults to undefined|


### Return type

**FetchPublications200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**400** | Error |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updatePublicationsV2ByTeamId**
> FetchPublications200Response updatePublicationsV2ByTeamId(updatePublicationsRequest)

Update publications by team id

### Example

```typescript
import {
    PublicationApi,
    Configuration,
    UpdatePublicationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //publication id (default to undefined)
let updatePublicationsRequest: UpdatePublicationsRequest; //Pass user credentials

const { status, data } = await apiInstance.updatePublicationsV2ByTeamId(
    teamId,
    id,
    updatePublicationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updatePublicationsRequest** | **UpdatePublicationsRequest**| Pass user credentials | |
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | publication id | defaults to undefined|


### Return type

**FetchPublications200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**400** | Error |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updatePublicationsV2ByUserId**
> FetchPublications200Response updatePublicationsV2ByUserId(updatePublicationsRequest)

Update publications by user id

### Example

```typescript
import {
    PublicationApi,
    Configuration,
    UpdatePublicationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new PublicationApi(configuration);

let userId: number; //ID of the user (default to undefined)
let id: number; //publication id (default to undefined)
let updatePublicationsRequest: UpdatePublicationsRequest; //Pass user credentials

const { status, data } = await apiInstance.updatePublicationsV2ByUserId(
    userId,
    id,
    updatePublicationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updatePublicationsRequest** | **UpdatePublicationsRequest**| Pass user credentials | |
| **userId** | [**number**] | ID of the user | defaults to undefined|
| **id** | [**number**] | publication id | defaults to undefined|


### Return type

**FetchPublications200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**400** | Error |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

