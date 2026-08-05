# PublicationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**countUniqueFieldsPublications**](#countuniquefieldspublications) | **GET** /api/v1/publication/count/{field} | PublicationController@count|
|[**createPublications**](#createpublications) | **POST** /api/v1/publications | PublicationController@store|
|[**deletePublications**](#deletepublications) | **DELETE** /api/v1/publications/{id} | PublicationController@destroy|
|[**editPublications**](#editpublications) | **PATCH** /api/v1/publications/{id} | PublicationController@edit|
|[**fetchAllPublications**](#fetchallpublications) | **GET** /api/v1/publications | PublicationController@index|
|[**fetchAllPublicationsV2**](#fetchallpublicationsv2) | **GET** /api/v2/publications | PublicationController@indexActive|
|[**fetchPublications**](#fetchpublications) | **GET** /api/v1/publications/{id} | PublicationController@show|
|[**fetchPublicationsV2**](#fetchpublicationsv2) | **GET** /api/v2/publications/{id} | PublicationController@showActive|
|[**updatePublications**](#updatepublications) | **PUT** /api/v1/publications/{id} | PublicationController@update|

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

# **createPublications**
> CreateDarIntegration201Response createPublications(createPublicationsRequest)

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

**CreateDarIntegration201Response**

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

