# CollectionsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**countUniqueFieldsCollections**](#countuniquefieldscollections) | **GET** /api/v1/collections/count/{field} | CollectionController@count|
|[**countUniqueFieldsCollectionsV2**](#countuniquefieldscollectionsv2) | **GET** /api/v2/collections/count/{field} | CollectionController@count|
|[**createCollections**](#createcollections) | **POST** /api/v2/collections | CollectionController@store|
|[**deleteCollectionsV2**](#deletecollectionsv2) | **DELETE** /api/v2/collections/{id} | Delete a collection|
|[**editCollectionsV2**](#editcollectionsv2) | **PATCH** /api/v2/collections/{id} | Edit a collection|
|[**fetchAllCollections**](#fetchallcollections) | **GET** /api/v1/collections | CollectionController@index|
|[**fetchAllCollectionsV2**](#fetchallcollectionsv2) | **GET** /api/v2/collections | CollectionController@index|
|[**fetchCollections**](#fetchcollections) | **GET** /api/v1/collections/{id} | CollectionController@show|
|[**fetchCollectionsV2**](#fetchcollectionsv2) | **GET** /api/v2/collections/{id} | CollectionController@show|
|[**updateCollectionsV2**](#updatecollectionsv2) | **PUT** /api/v2/collections/{id} | Update a collection|

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

# **createCollections**
> CreateDarIntegration201Response createCollections(createCollectionsRequest)

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

# **deleteCollectionsV2**
> DeleteApplications200Response deleteCollectionsV2()

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

