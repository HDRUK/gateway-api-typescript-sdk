# SearchSimilarDatasetsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**searchSimilarDatasets**](#searchsimilardatasets) | **POST** /api/v1/search/similar/datasets | Search@similarDatasets|

# **searchSimilarDatasets**
> SearchSimilarDatasets200Response searchSimilarDatasets(searchSimilarDatasetsRequest)

Returns top three gateway datasets most similar to the provided dataset

### Example

```typescript
import {
    SearchSimilarDatasetsApi,
    Configuration,
    SearchSimilarDatasetsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new SearchSimilarDatasetsApi(configuration);

let searchSimilarDatasetsRequest: SearchSimilarDatasetsRequest; //Submit dataset id

const { status, data } = await apiInstance.searchSimilarDatasets(
    searchSimilarDatasetsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **searchSimilarDatasetsRequest** | **SearchSimilarDatasetsRequest**| Submit dataset id | |


### Return type

**SearchSimilarDatasets200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

