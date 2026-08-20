# DatasetLinkCheckResultsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**fetchDatasetLinkCheckResultsV2**](#fetchdatasetlinkcheckresultsv2) | **GET** /api/v2/dataset_link_check_results | DatasetLinkCheckResultController@index|

# **fetchDatasetLinkCheckResultsV2**
> FetchDatasetLinkCheckResultsV2200Response fetchDatasetLinkCheckResultsV2()

Get the confirmed dead links (HTTP 404, verified across multiple checks) found in active dataset metadata by the nightly link check

### Example

```typescript
import {
    DatasetLinkCheckResultsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetLinkCheckResultsApi(configuration);

const { status, data } = await apiInstance.fetchDatasetLinkCheckResultsV2();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**FetchDatasetLinkCheckResultsV2200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

