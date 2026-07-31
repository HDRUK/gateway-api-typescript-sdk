# WorkgroupsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**fetchAllWorkgroups**](#fetchallworkgroups) | **GET** /api/v1/workgroups | WorkgroupController@index|

# **fetchAllWorkgroups**
> FetchAllWorkgroups200Response fetchAllWorkgroups()

Get All Workgroups

### Example

```typescript
import {
    WorkgroupsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new WorkgroupsApi(configuration);

const { status, data } = await apiInstance.fetchAllWorkgroups();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**FetchAllWorkgroups200Response**

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

