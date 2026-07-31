# SearchDatasetsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**searchDatasets**](#searchdatasets) | **POST** /api/v1/search/datasets | Search@datasets|

# **searchDatasets**
> SearchDatasets200Response searchDatasets(searchDatasetsRequest)

Returns gateway datasets related to the provided query term(s)

### Example

```typescript
import {
    SearchDatasetsApi,
    Configuration,
    SearchDatasetsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new SearchDatasetsApi(configuration);

let searchDatasetsRequest: SearchDatasetsRequest; //Submit search query

const { status, data } = await apiInstance.searchDatasets(
    searchDatasetsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **searchDatasetsRequest** | **SearchDatasetsRequest**| Submit search query | |


### Return type

**SearchDatasets200Response**

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

