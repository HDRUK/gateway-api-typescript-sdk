# IntegrationCollectionsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createCollectionsIntegrations**](#createcollectionsintegrations) | **POST** /api/v1/integrations/collections | IntegrationCollectionController@store|
|[**deleteCollectionsIntegrations**](#deletecollectionsintegrations) | **DELETE** /api/v1/integrations/collections/{id} | Delete a collection|
|[**editCollectionsIntegrations**](#editcollectionsintegrations) | **PATCH** /api/v1/integrations/collections/{id} | Edit a collection|
|[**fetchAllCollectionsIntegrations**](#fetchallcollectionsintegrations) | **GET** /api/v1/integrations/collections | IntegrationCollectionController@index|
|[**fetchCollectionsIntegrations**](#fetchcollectionsintegrations) | **GET** /api/v1/integrations/collections/{id} | IntegrationCollectionController@show|
|[**updateCollectionsIntegrations**](#updatecollectionsintegrations) | **PUT** /api/v1/integrations/collections/{id} | Update a collection|

# **createCollectionsIntegrations**
> CreateCategories200Response createCollectionsIntegrations(updateTeamCollectionsRequest)

Create a new collection

### Example

```typescript
import {
    IntegrationCollectionsApi,
    Configuration,
    UpdateTeamCollectionsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new IntegrationCollectionsApi(configuration);

let updateTeamCollectionsRequest: UpdateTeamCollectionsRequest; //Pass user credentials

const { status, data } = await apiInstance.createCollectionsIntegrations(
    updateTeamCollectionsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateTeamCollectionsRequest** | **UpdateTeamCollectionsRequest**| Pass user credentials | |


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

# **deleteCollectionsIntegrations**
> DeleteAliases200Response deleteCollectionsIntegrations()

Delete a collection

### Example

```typescript
import {
    IntegrationCollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new IntegrationCollectionsApi(configuration);

let id: number; //collection id (default to undefined)

const { status, data } = await apiInstance.deleteCollectionsIntegrations(
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

# **editCollectionsIntegrations**
> FetchCollections200Response editCollectionsIntegrations(updateTeamCollectionsRequest)

Edit a collection

### Example

```typescript
import {
    IntegrationCollectionsApi,
    Configuration,
    UpdateTeamCollectionsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new IntegrationCollectionsApi(configuration);

let id: number; //collection id (default to undefined)
let updateTeamCollectionsRequest: UpdateTeamCollectionsRequest; //Pass user credentials

const { status, data } = await apiInstance.editCollectionsIntegrations(
    id,
    updateTeamCollectionsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateTeamCollectionsRequest** | **UpdateTeamCollectionsRequest**| Pass user credentials | |
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

# **fetchAllCollectionsIntegrations**
> FetchAllCollections200Response fetchAllCollectionsIntegrations()

Returns a list of collections

### Example

```typescript
import {
    IntegrationCollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new IntegrationCollectionsApi(configuration);

let name: string; //Filter collections by name (optional) (default to undefined)
let perPage: number; //per page (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllCollectionsIntegrations(
    name,
    perPage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **name** | [**string**] | Filter collections by name | (optional) defaults to undefined|
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

# **fetchCollectionsIntegrations**
> FetchCollections200Response fetchCollectionsIntegrations()

Get collection by id

### Example

```typescript
import {
    IntegrationCollectionsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new IntegrationCollectionsApi(configuration);

let id: number; //collection id (default to undefined)

const { status, data } = await apiInstance.fetchCollectionsIntegrations(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
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

# **updateCollectionsIntegrations**
> FetchCollections200Response updateCollectionsIntegrations(updateTeamCollectionsRequest)

Update a collection

### Example

```typescript
import {
    IntegrationCollectionsApi,
    Configuration,
    UpdateTeamCollectionsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new IntegrationCollectionsApi(configuration);

let id: number; //collection id (default to undefined)
let updateTeamCollectionsRequest: UpdateTeamCollectionsRequest; //Pass user credentials

const { status, data } = await apiInstance.updateCollectionsIntegrations(
    id,
    updateTeamCollectionsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateTeamCollectionsRequest** | **UpdateTeamCollectionsRequest**| Pass user credentials | |
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

