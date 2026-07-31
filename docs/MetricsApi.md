# MetricsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**fetchKeyMetricsV2**](#fetchkeymetricsv2) | **GET** /api/v2/metrics | KeyMetricController@index|

# **fetchKeyMetricsV2**
> FetchKeyMetricsV2200Response fetchKeyMetricsV2()

Get key metrics

### Example

```typescript
import {
    MetricsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new MetricsApi(configuration);

const { status, data } = await apiInstance.fetchKeyMetricsV2();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**FetchKeyMetricsV2200Response**

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

