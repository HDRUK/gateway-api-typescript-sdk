# NightlyDatasetTestsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**fetchNightlyDatasetTestsV2**](#fetchnightlydatasettestsv2) | **GET** /api/v2/nightly_dataset_tests | NightlyDatasetTestController@index|

# **fetchNightlyDatasetTestsV2**
> FetchDatasetLinkCheckResultsV2200Response fetchNightlyDatasetTestsV2()

Get the results of the nightly dataset reachability check, with a summary and a list of failures

### Example

```typescript
import {
    NightlyDatasetTestsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new NightlyDatasetTestsApi(configuration);

const { status, data } = await apiInstance.fetchNightlyDatasetTestsV2();
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

