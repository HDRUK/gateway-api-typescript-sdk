# SavedSearchApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createSavedSearches**](#createsavedsearches) | **POST** /api/v1/saved_searches | SavedSearch@store|
|[**deleteSavedSearches**](#deletesavedsearches) | **DELETE** /api/v1/saved_searches/{id} | SavedSearch@destroy|
|[**editSavedSearches**](#editsavedsearches) | **PATCH** /api/v1/saved_searches/{id} | SavedSearch@update|
|[**fetchAllSavedSearches**](#fetchallsavedsearches) | **GET** /api/v1/saved_searches | SavedSearch@index|
|[**fetchSavedSearches**](#fetchsavedsearches) | **GET** /api/v1/saved_searches/{id} | SavedSearch@show|
|[**updateSavedSearches**](#updatesavedsearches) | **PUT** /api/v1/saved_searches/{id} | SavedSearch@update|

# **createSavedSearches**
> CreateCategories200Response createSavedSearches(createSavedSearchesRequest)

Creates a new saved search

### Example

```typescript
import {
    SavedSearchApi,
    Configuration,
    CreateSavedSearchesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new SavedSearchApi(configuration);

let createSavedSearchesRequest: CreateSavedSearchesRequest; //Saved search definition

const { status, data } = await apiInstance.createSavedSearches(
    createSavedSearchesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createSavedSearchesRequest** | **CreateSavedSearchesRequest**| Saved search definition | |


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
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteSavedSearches**
> DeleteAliases200Response deleteSavedSearches()

Delete a saved search

### Example

```typescript
import {
    SavedSearchApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new SavedSearchApi(configuration);

let id: number; //saved search id (default to undefined)

const { status, data } = await apiInstance.deleteSavedSearches(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | saved search id | defaults to undefined|


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

# **editSavedSearches**
> UpdateSavedSearches200Response editSavedSearches(editSavedSearchesRequest)

Edit a saved search

### Example

```typescript
import {
    SavedSearchApi,
    Configuration,
    EditSavedSearchesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new SavedSearchApi(configuration);

let id: number; //saved search id (default to undefined)
let editSavedSearchesRequest: EditSavedSearchesRequest; //Saved search definition

const { status, data } = await apiInstance.editSavedSearches(
    id,
    editSavedSearchesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editSavedSearchesRequest** | **EditSavedSearchesRequest**| Saved search definition | |
| **id** | [**number**] | saved search id | defaults to undefined|


### Return type

**UpdateSavedSearches200Response**

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

# **fetchAllSavedSearches**
> FetchAllSavedSearches200Response fetchAllSavedSearches()

Returns a list of saved searches enabled on the system

### Example

```typescript
import {
    SavedSearchApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new SavedSearchApi(configuration);

let perPage: number; //Specify number of results per page (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllSavedSearches(
    perPage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **perPage** | [**number**] | Specify number of results per page | (optional) defaults to undefined|


### Return type

**FetchAllSavedSearches200Response**

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

# **fetchSavedSearches**
> FetchAllSavedSearches200Response fetchSavedSearches()

Return a single saved search

### Example

```typescript
import {
    SavedSearchApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new SavedSearchApi(configuration);

let id: number; //saved search id (default to undefined)

const { status, data } = await apiInstance.fetchSavedSearches(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | saved search id | defaults to undefined|


### Return type

**FetchAllSavedSearches200Response**

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

# **updateSavedSearches**
> UpdateSavedSearches200Response updateSavedSearches(updateSavedSearchesRequest)

Update a saved search

### Example

```typescript
import {
    SavedSearchApi,
    Configuration,
    UpdateSavedSearchesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new SavedSearchApi(configuration);

let id: number; //saved search id (default to undefined)
let updateSavedSearchesRequest: UpdateSavedSearchesRequest; //Saved search definition

const { status, data } = await apiInstance.updateSavedSearches(
    id,
    updateSavedSearchesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateSavedSearchesRequest** | **UpdateSavedSearchesRequest**| Saved search definition | |
| **id** | [**number**] | saved search id | defaults to undefined|


### Return type

**UpdateSavedSearches200Response**

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

