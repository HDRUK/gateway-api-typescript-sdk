# CollectionsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**countTeamUniqueFieldsCollectionV2**](#countteamuniquefieldscollectionv2) | **GET** /api/v2/teams/{teamId}/collections/count/{field} | TeamCollectionController@count|
|[**countUniqueFieldsCollections**](#countuniquefieldscollections) | **GET** /api/v1/collections/count/{field} | CollectionController@count|
|[**countUniqueFieldsCollectionsV2**](#countuniquefieldscollectionsv2) | **GET** /api/v2/collections/count/{field} | CollectionController@count|
|[**countUserUniqueFieldsCollectionV2**](#countuseruniquefieldscollectionv2) | **GET** /api/v2/users/{userId}/collections/count/{field} | UserCollectionController@count|
|[**createCollections**](#createcollections) | **POST** /api/v2/collections | CollectionController@store|
|[**createTeamCollections**](#createteamcollections) | **POST** /api/v1/teams/{teamId}/collections | CollectionController@store|
|[**createTeamCollectionsV2**](#createteamcollectionsv2) | **POST** /api/v2/teams/{teamId}/collections | TeamCollectionController@store|
|[**createUserCollections**](#createusercollections) | **POST** /api/v2/users/collections | UserCollectionController@store|
|[**deleteCollectionsV2**](#deletecollectionsv2) | **DELETE** /api/v2/collections/{id} | Delete a collection|
|[**deleteTeamCollections**](#deleteteamcollections) | **DELETE** /api/v1/teams/{teamId}/collections/{id} | Delete a collection|
|[**deleteTeamCollectionsV2**](#deleteteamcollectionsv2) | **DELETE** /api/v2/teams/{teamId}/collections/{id} | Delete a collection|
|[**deleteUserCollectionsV2**](#deleteusercollectionsv2) | **DELETE** /api/v2/users/{userId}/collections/{id} | Delete a collection|
|[**editCollectionsV2**](#editcollectionsv2) | **PATCH** /api/v2/collections/{id} | Edit a collection|
|[**editTeamCollections**](#editteamcollections) | **PATCH** /api/v1/teams/{teamId}/collections/{id} | Edit a collection|
|[**editTeamCollectionsV2**](#editteamcollectionsv2) | **PATCH** /api/v2/teams/{teamId}/collections/{id} | Edit a collection|
|[**editUserCollectionsV2**](#editusercollectionsv2) | **PATCH** /api/v2/users/{userId}/collections/{id} | Edit a collection|
|[**fetchAllCollections**](#fetchallcollections) | **GET** /api/v1/collections | CollectionController@index|
|[**fetchAllCollectionsV2**](#fetchallcollectionsv2) | **GET** /api/v2/collections | CollectionController@index|
|[**fetchCollections**](#fetchcollections) | **GET** /api/v1/collections/{id} | CollectionController@show|
|[**fetchCollectionsV2**](#fetchcollectionsv2) | **GET** /api/v2/collections/{id} | CollectionController@show|
|[**fetchTeamActiveCollectionsV2**](#fetchteamactivecollectionsv2) | **GET** /api/v2/teams/{teamId}/collections/status/active | TeamCollectionController@indexActive|
|[**fetchTeamArchivedCollectionsV2**](#fetchteamarchivedcollectionsv2) | **GET** /api/v2/teams/{teamId}/collections/status/archived | TeamCollectionController@indexArchived|
|[**fetchTeamCollectionV2**](#fetchteamcollectionv2) | **GET** /api/v2/teams/{teamId}/collections/{id} | TeamCollectionController@show|
|[**fetchTeamDraftCollectionsV2**](#fetchteamdraftcollectionsv2) | **GET** /api/v2/teams/{teamId}/collections/status/draft | TeamCollectionController@indexDraft|
|[**fetchUserArchivedCollectionsV2**](#fetchuserarchivedcollectionsv2) | **GET** /api/v2/users/{userId}/collections/status/archived | UserCollectionController@indexArchived|
|[**fetchUserCollectionV2**](#fetchusercollectionv2) | **GET** /api/v2/users/{userId}/collections/{id} | CollectionController@show|
|[**fetchUserCollectionsV2**](#fetchusercollectionsv2) | **GET** /api/v2/users/{userId}/collections/status/active | UserCollectionController@indexActive|
|[**fetchUserDraftCollectionsV2**](#fetchuserdraftcollectionsv2) | **GET** /api/v2/users/{userId}/collections/status/draft | UserCollectionController@indexDraft|
|[**updateCollectionsV2**](#updatecollectionsv2) | **PUT** /api/v2/collections/{id} | Update a collection|
|[**updateTeamCollections**](#updateteamcollections) | **PUT** /api/v1/teams/{teamId}/collections/{id} | Update a collection|
|[**updateTeamCollectionsV2**](#updateteamcollectionsv2) | **PUT** /api/v2/teams/{teamId}/collections/{id} | Update a collection|
|[**updateUserCollectionsV2**](#updateusercollectionsv2) | **PUT** /api/v2/users/{userId}/collections/{id} | Update a collection|

# **countTeamUniqueFieldsCollectionV2**
> CountUniqueFieldsCollections200Response countTeamUniqueFieldsCollectionV2()

Get user counts for distinct entries of a field in the model

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let teamId: number; //team id (default to undefined)
let field: string; //name of the field to perform a count on (default to undefined)

const { status, data } = await apiInstance.countTeamUniqueFieldsCollectionV2(
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

# **countUniqueFieldsCollections**
> CountUniqueFieldsCollections200Response countUniqueFieldsCollections()

Get Counts for distinct entries of a field in the model

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let field: string; //name of the field to perform a count on (default to undefined)
let teamId: number; //team id (default to undefined)
let userId: number; //user id (default to undefined)

const { status, data } = await apiInstance.countUniqueFieldsCollections(
    field,
    teamId,
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **field** | [**string**] | name of the field to perform a count on | defaults to undefined|
| **teamId** | [**number**] | team id | defaults to undefined|
| **userId** | [**number**] | user id | defaults to undefined|


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

# **countUniqueFieldsCollectionsV2**
> CountUniqueFieldsCollections200Response countUniqueFieldsCollectionsV2()

Get Counts for distinct entries of a field in the model

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let field: string; //name of the field to perform a count on (default to undefined)

const { status, data } = await apiInstance.countUniqueFieldsCollectionsV2(
    field
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
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

# **countUserUniqueFieldsCollectionV2**
> CountUniqueFieldsCollections200Response countUserUniqueFieldsCollectionV2()

Get user counts for distinct entries of a field in the model

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let userId: number; //user id (default to undefined)
let field: string; //name of the field to perform a count on (default to undefined)

const { status, data } = await apiInstance.countUserUniqueFieldsCollectionV2(
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

# **createCollections**
> CreateCategories200Response createCollections(createCollectionsRequest)

Create a new collection owned by an individual

### Example

```typescript
import {
    CollectionsApi,
    Configuration,
    CreateCollectionsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let createCollectionsRequest: CreateCollectionsRequest; //Pass user credentials

const { status, data } = await apiInstance.createCollections(
    createCollectionsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createCollectionsRequest** | **CreateCollectionsRequest**| Pass user credentials | |


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

# **createTeamCollections**
> CreateCategories200Response createTeamCollections(createTeamCollectionsRequest)

Create a new collection for a team

### Example

```typescript
import {
    CollectionsApi,
    Configuration,
    CreateTeamCollectionsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let teamId: number; //team id (default to undefined)
let createTeamCollectionsRequest: CreateTeamCollectionsRequest; //Pass user credentials

const { status, data } = await apiInstance.createTeamCollections(
    teamId,
    createTeamCollectionsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createTeamCollectionsRequest** | **CreateTeamCollectionsRequest**| Pass user credentials | |
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

# **createTeamCollectionsV2**
> CreateCategories200Response createTeamCollectionsV2(createTeamCollectionsRequest)

Create a new collection for a team

### Example

```typescript
import {
    CollectionsApi,
    Configuration,
    CreateTeamCollectionsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let teamId: number; //team id (default to undefined)
let createTeamCollectionsRequest: CreateTeamCollectionsRequest; //Pass user credentials

const { status, data } = await apiInstance.createTeamCollectionsV2(
    teamId,
    createTeamCollectionsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createTeamCollectionsRequest** | **CreateTeamCollectionsRequest**| Pass user credentials | |
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

# **createUserCollections**
> CreateCategories200Response createUserCollections(createCollectionsRequest)

Create a new collection owned by an individual

### Example

```typescript
import {
    CollectionsApi,
    Configuration,
    CreateCollectionsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let createCollectionsRequest: CreateCollectionsRequest; //Pass user credentials

const { status, data } = await apiInstance.createUserCollections(
    createCollectionsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createCollectionsRequest** | **CreateCollectionsRequest**| Pass user credentials | |


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

# **deleteCollectionsV2**
> DeleteAliases200Response deleteCollectionsV2()

Delete a collection

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let id: number; //collection id (default to undefined)

const { status, data } = await apiInstance.deleteCollectionsV2(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | collection id | defaults to undefined|


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

# **deleteTeamCollections**
> DeleteAliases200Response deleteTeamCollections()

Delete a collection owned by a team

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //collection id (default to undefined)

const { status, data } = await apiInstance.deleteTeamCollections(
    teamId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | collection id | defaults to undefined|


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

# **deleteTeamCollectionsV2**
> DeleteAliases200Response deleteTeamCollectionsV2()

Delete a collection owned by a team

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //collection id (default to undefined)

const { status, data } = await apiInstance.deleteTeamCollectionsV2(
    teamId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | collection id | defaults to undefined|


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

# **deleteUserCollectionsV2**
> DeleteAliases200Response deleteUserCollectionsV2()

Delete a collection

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let userId: number; //user id (default to undefined)
let id: number; //collection id (default to undefined)

const { status, data } = await apiInstance.deleteUserCollectionsV2(
    userId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | user id | defaults to undefined|
| **id** | [**number**] | collection id | defaults to undefined|


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

# **editCollectionsV2**
> FetchCollections200Response editCollectionsV2(editCollectionsV2Request)

Edit a collection

### Example

```typescript
import {
    CollectionsApi,
    Configuration,
    EditCollectionsV2Request
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let id: number; //collection id (default to undefined)
let editCollectionsV2Request: EditCollectionsV2Request; //Pass user credentials
let unarchive: string; //Unarchive a collection (optional) (default to undefined)

const { status, data } = await apiInstance.editCollectionsV2(
    id,
    editCollectionsV2Request,
    unarchive
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editCollectionsV2Request** | **EditCollectionsV2Request**| Pass user credentials | |
| **id** | [**number**] | collection id | defaults to undefined|
| **unarchive** | [**string**] | Unarchive a collection | (optional) defaults to undefined|


### Return type

**FetchCollections200Response**

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

# **editTeamCollections**
> FetchCollections200Response editTeamCollections(editTeamCollectionsRequest)

Edit a collection owned by a team

### Example

```typescript
import {
    CollectionsApi,
    Configuration,
    EditTeamCollectionsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //collection id (default to undefined)
let editTeamCollectionsRequest: EditTeamCollectionsRequest; //Pass user credentials
let unarchive: string; //Unarchive a collection (optional) (default to undefined)

const { status, data } = await apiInstance.editTeamCollections(
    teamId,
    id,
    editTeamCollectionsRequest,
    unarchive
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editTeamCollectionsRequest** | **EditTeamCollectionsRequest**| Pass user credentials | |
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | collection id | defaults to undefined|
| **unarchive** | [**string**] | Unarchive a collection | (optional) defaults to undefined|


### Return type

**FetchCollections200Response**

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

# **editTeamCollectionsV2**
> FetchCollections200Response editTeamCollectionsV2(editTeamCollectionsRequest)

Edit a collection owned by a team

### Example

```typescript
import {
    CollectionsApi,
    Configuration,
    EditTeamCollectionsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //collection id (default to undefined)
let editTeamCollectionsRequest: EditTeamCollectionsRequest; //Pass user credentials

const { status, data } = await apiInstance.editTeamCollectionsV2(
    teamId,
    id,
    editTeamCollectionsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editTeamCollectionsRequest** | **EditTeamCollectionsRequest**| Pass user credentials | |
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | collection id | defaults to undefined|


### Return type

**FetchCollections200Response**

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

# **editUserCollectionsV2**
> FetchCollections200Response editUserCollectionsV2(editCollectionsV2Request)

Edit a collection

### Example

```typescript
import {
    CollectionsApi,
    Configuration,
    EditCollectionsV2Request
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let userId: number; //user id (default to undefined)
let id: number; //collection id (default to undefined)
let editCollectionsV2Request: EditCollectionsV2Request; //Pass user credentials

const { status, data } = await apiInstance.editUserCollectionsV2(
    userId,
    id,
    editCollectionsV2Request
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editCollectionsV2Request** | **EditCollectionsV2Request**| Pass user credentials | |
| **userId** | [**number**] | user id | defaults to undefined|
| **id** | [**number**] | collection id | defaults to undefined|


### Return type

**FetchCollections200Response**

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

# **fetchAllCollections**
> FetchAllCollections200Response fetchAllCollections()

Returns a list of collections

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let name: string; //Filter collections by name (optional) (default to undefined)
let teamId: number; //Filter collections by team ID (optional) (default to undefined)
let userId: number; //Filter collections by user ID (optional) (default to undefined)
let title: string; //Filter collections by title (optional) (default to undefined)
let status: string; //Filter collections by status (DRAFT, ACTIVE, ARCHIVED) (optional) (default to undefined)
let perPage: number; //per page (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllCollections(
    name,
    teamId,
    userId,
    title,
    status,
    perPage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **name** | [**string**] | Filter collections by name | (optional) defaults to undefined|
| **teamId** | [**number**] | Filter collections by team ID | (optional) defaults to undefined|
| **userId** | [**number**] | Filter collections by user ID | (optional) defaults to undefined|
| **title** | [**string**] | Filter collections by title | (optional) defaults to undefined|
| **status** | [**string**] | Filter collections by status (DRAFT, ACTIVE, ARCHIVED) | (optional) defaults to undefined|
| **perPage** | [**number**] | per page | (optional) defaults to undefined|


### Return type

**FetchAllCollections200Response**

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

# **fetchAllCollectionsV2**
> FetchAllCollections200Response fetchAllCollectionsV2()

Returns a list of collections

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

const { status, data } = await apiInstance.fetchAllCollectionsV2();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**FetchAllCollections200Response**

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

# **fetchCollections**
> FetchCollections200Response fetchCollections()

Get collection by id

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let id: number; //collection id (default to undefined)
let viewType: string; //Query flag to show full collection data or a trimmed version (defaults to full). (optional) (default to 'full')

const { status, data } = await apiInstance.fetchCollections(
    id,
    viewType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | collection id | defaults to undefined|
| **viewType** | [**string**] | Query flag to show full collection data or a trimmed version (defaults to full). | (optional) defaults to 'full'|


### Return type

**FetchCollections200Response**

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

# **fetchCollectionsV2**
> FetchCollections200Response fetchCollectionsV2()

Get collection by id

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let id: number; //collection id (default to undefined)
let viewType: string; //Query flag to show full collection data or a trimmed version (defaults to full). (optional) (default to 'full')

const { status, data } = await apiInstance.fetchCollectionsV2(
    id,
    viewType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | collection id | defaults to undefined|
| **viewType** | [**string**] | Query flag to show full collection data or a trimmed version (defaults to full). | (optional) defaults to 'full'|


### Return type

**FetchCollections200Response**

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

# **fetchTeamActiveCollectionsV2**
> FetchAllCollections200Response fetchTeamActiveCollectionsV2()

Returns a list of a teams collections

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let teamId: number; //team id (default to undefined)

const { status, data } = await apiInstance.fetchTeamActiveCollectionsV2(
    teamId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|


### Return type

**FetchAllCollections200Response**

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

# **fetchTeamArchivedCollectionsV2**
> FetchAllCollections200Response fetchTeamArchivedCollectionsV2()

Returns a list of a teams archived collections

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let teamId: number; //team id (default to undefined)

const { status, data } = await apiInstance.fetchTeamArchivedCollectionsV2(
    teamId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|


### Return type

**FetchAllCollections200Response**

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

# **fetchTeamCollectionV2**
> FetchCollections200Response fetchTeamCollectionV2()

Get collection by id

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //collection id (default to undefined)

const { status, data } = await apiInstance.fetchTeamCollectionV2(
    teamId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | collection id | defaults to undefined|


### Return type

**FetchCollections200Response**

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

# **fetchTeamDraftCollectionsV2**
> FetchAllCollections200Response fetchTeamDraftCollectionsV2()

Returns a list of a teams draft collections

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let teamId: number; //team id (default to undefined)

const { status, data } = await apiInstance.fetchTeamDraftCollectionsV2(
    teamId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|


### Return type

**FetchAllCollections200Response**

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

# **fetchUserArchivedCollectionsV2**
> FetchAllCollections200Response fetchUserArchivedCollectionsV2()

Returns a list of a users archived collections

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let userId: number; //user id (default to undefined)

const { status, data } = await apiInstance.fetchUserArchivedCollectionsV2(
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | user id | defaults to undefined|


### Return type

**FetchAllCollections200Response**

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

# **fetchUserCollectionV2**
> FetchCollections200Response fetchUserCollectionV2()

Get collection by id

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let userId: number; //user id (default to undefined)
let id: number; //collection id (default to undefined)

const { status, data } = await apiInstance.fetchUserCollectionV2(
    userId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | user id | defaults to undefined|
| **id** | [**number**] | collection id | defaults to undefined|


### Return type

**FetchCollections200Response**

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

# **fetchUserCollectionsV2**
> FetchAllCollections200Response fetchUserCollectionsV2()

Returns a list of a users collections

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let userId: number; //user id (default to undefined)

const { status, data } = await apiInstance.fetchUserCollectionsV2(
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | user id | defaults to undefined|


### Return type

**FetchAllCollections200Response**

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

# **fetchUserDraftCollectionsV2**
> FetchAllCollections200Response fetchUserDraftCollectionsV2()

Returns a list of a users draft collections

### Example

```typescript
import {
    CollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let userId: number; //user id (default to undefined)

const { status, data } = await apiInstance.fetchUserDraftCollectionsV2(
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | user id | defaults to undefined|


### Return type

**FetchAllCollections200Response**

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

# **updateCollectionsV2**
> FetchCollections200Response updateCollectionsV2(updateCollectionsV2Request)

Update a collection owned by an individual

### Example

```typescript
import {
    CollectionsApi,
    Configuration,
    UpdateCollectionsV2Request
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let id: number; //collection id (default to undefined)
let updateCollectionsV2Request: UpdateCollectionsV2Request; //Pass user credentials

const { status, data } = await apiInstance.updateCollectionsV2(
    id,
    updateCollectionsV2Request
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateCollectionsV2Request** | **UpdateCollectionsV2Request**| Pass user credentials | |
| **id** | [**number**] | collection id | defaults to undefined|


### Return type

**FetchCollections200Response**

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

# **updateTeamCollections**
> FetchCollections200Response updateTeamCollections(updateTeamCollectionsRequest)

Update a collection owned by a team

### Example

```typescript
import {
    CollectionsApi,
    Configuration,
    UpdateTeamCollectionsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //collection id (default to undefined)
let updateTeamCollectionsRequest: UpdateTeamCollectionsRequest; //Pass user credentials

const { status, data } = await apiInstance.updateTeamCollections(
    teamId,
    id,
    updateTeamCollectionsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateTeamCollectionsRequest** | **UpdateTeamCollectionsRequest**| Pass user credentials | |
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | collection id | defaults to undefined|


### Return type

**FetchCollections200Response**

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

# **updateTeamCollectionsV2**
> FetchCollections200Response updateTeamCollectionsV2(updateTeamCollectionsRequest)

Update a collection owned by a team

### Example

```typescript
import {
    CollectionsApi,
    Configuration,
    UpdateTeamCollectionsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //collection id (default to undefined)
let updateTeamCollectionsRequest: UpdateTeamCollectionsRequest; //Pass user credentials

const { status, data } = await apiInstance.updateTeamCollectionsV2(
    teamId,
    id,
    updateTeamCollectionsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateTeamCollectionsRequest** | **UpdateTeamCollectionsRequest**| Pass user credentials | |
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | collection id | defaults to undefined|


### Return type

**FetchCollections200Response**

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

# **updateUserCollectionsV2**
> FetchCollections200Response updateUserCollectionsV2(updateCollectionsV2Request)

Update a collection owned by an individual

### Example

```typescript
import {
    CollectionsApi,
    Configuration,
    UpdateCollectionsV2Request
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CollectionsApi(configuration);

let userId: number; //user id (default to undefined)
let id: number; //collection id (default to undefined)
let updateCollectionsV2Request: UpdateCollectionsV2Request; //Pass user credentials

const { status, data } = await apiInstance.updateUserCollectionsV2(
    userId,
    id,
    updateCollectionsV2Request
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateCollectionsV2Request** | **UpdateCollectionsV2Request**| Pass user credentials | |
| **userId** | [**number**] | user id | defaults to undefined|
| **id** | [**number**] | collection id | defaults to undefined|


### Return type

**FetchCollections200Response**

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

