# SearchPublicationsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**searchPublications**](#searchpublications) | **POST** /api/v1/search/publications | Search@publications|
|[**searchPublicationsByDoi**](#searchpublicationsbydoi) | **POST** /api/v1/search/doi | Search@publications|

# **searchPublications**
> SearchPublications200Response searchPublications(searchPublicationsRequest)

Returns gateway publications related to the provided query term(s)

### Example

```typescript
import {
    SearchPublicationsApi,
    Configuration,
    SearchPublicationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new SearchPublicationsApi(configuration);

let searchPublicationsRequest: SearchPublicationsRequest; //Submit search query
let sort: string; //Field to sort by (default: \'score\') (optional) (default to undefined)
let direction: 'asc' | 'desc'; //Sort direction (\'asc\' or \'desc\', default: \'desc\') (optional) (default to undefined)
let source: 'GAT' | 'FED'; //Which source to search (\'GAT\' or \'FED\', default: \'GAT\') (optional) (default to undefined)

const { status, data } = await apiInstance.searchPublications(
    searchPublicationsRequest,
    sort,
    direction,
    source
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **searchPublicationsRequest** | **SearchPublicationsRequest**| Submit search query | |
| **sort** | [**string**] | Field to sort by (default: \&#39;score\&#39;) | (optional) defaults to undefined|
| **direction** | [**&#39;asc&#39; | &#39;desc&#39;**]**Array<&#39;asc&#39; &#124; &#39;desc&#39;>** | Sort direction (\&#39;asc\&#39; or \&#39;desc\&#39;, default: \&#39;desc\&#39;) | (optional) defaults to undefined|
| **source** | [**&#39;GAT&#39; | &#39;FED&#39;**]**Array<&#39;GAT&#39; &#124; &#39;FED&#39;>** | Which source to search (\&#39;GAT\&#39; or \&#39;FED\&#39;, default: \&#39;GAT\&#39;) | (optional) defaults to undefined|


### Return type

**SearchPublications200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **searchPublicationsByDoi**
> SearchPublicationsByDoi200Response searchPublicationsByDoi(searchPublicationsByDoiRequest)

Returns publications from EuropePMC matching a give DOI

### Example

```typescript
import {
    SearchPublicationsApi,
    Configuration,
    SearchPublicationsByDoiRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new SearchPublicationsApi(configuration);

let searchPublicationsByDoiRequest: SearchPublicationsByDoiRequest; //Submit search query

const { status, data } = await apiInstance.searchPublicationsByDoi(
    searchPublicationsByDoiRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **searchPublicationsByDoiRequest** | **SearchPublicationsByDoiRequest**| Submit search query | |


### Return type

**SearchPublicationsByDoi200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**204** | No match found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

