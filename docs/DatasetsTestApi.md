# DatasetsTestApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**datasetsTest**](#datasetstest) | **POST** /api/v1/datasets/test | DatasetController@datasetTest|

# **datasetsTest**
> CreateCategories200Response datasetsTest(datasetsTestRequest)

Datasets test

### Example

```typescript
import {
    DatasetsTestApi,
    Configuration,
    DatasetsTestRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsTestApi(configuration);

let datasetsTestRequest: DatasetsTestRequest; //Pass datasets payload

const { status, data } = await apiInstance.datasetsTest(
    datasetsTestRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **datasetsTestRequest** | **DatasetsTestRequest**| Pass datasets payload | |


### Return type

**CreateCategories200Response**

### Authorization

No authorization required

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

