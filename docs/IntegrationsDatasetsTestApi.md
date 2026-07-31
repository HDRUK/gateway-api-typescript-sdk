# IntegrationsDatasetsTestApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**integrationsDatasetsTest**](#integrationsdatasetstest) | **POST** /api/v1/integrations/datasets/test | IntegrationDatasetController@datasetTest|

# **integrationsDatasetsTest**
> CreateCategories200Response integrationsDatasetsTest(datasetsTestRequest)

Integrations datasets test

### Example

```typescript
import {
    IntegrationsDatasetsTestApi,
    Configuration,
    DatasetsTestRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new IntegrationsDatasetsTestApi(configuration);

let datasetsTestRequest: DatasetsTestRequest; //Pass datasets payload

const { status, data } = await apiInstance.integrationsDatasetsTest(
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

