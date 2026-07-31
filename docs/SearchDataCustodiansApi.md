# SearchDataCustodiansApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**searchDataCustodians**](#searchdatacustodians) | **POST** /api/v1/search/data_custodians | Search@data_custodians|

# **searchDataCustodians**
> SearchDataCustodians200Response searchDataCustodians(searchDataCustodiansRequest)

Returns gateway data custodians related to the provided query term(s)

### Example

```typescript
import {
    SearchDataCustodiansApi,
    Configuration,
    SearchDataCustodiansRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new SearchDataCustodiansApi(configuration);

let searchDataCustodiansRequest: SearchDataCustodiansRequest; //Submit search query
let sort: string; //Field to sort by (default: \'score\') (optional) (default to undefined)
let direction: 'asc' | 'desc'; //Sort direction (\'asc\' or \'desc\', default: \'desc\') (optional) (default to undefined)
let perPage: number; //Number of results to return per page (optional) (default to undefined)

const { status, data } = await apiInstance.searchDataCustodians(
    searchDataCustodiansRequest,
    sort,
    direction,
    perPage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **searchDataCustodiansRequest** | **SearchDataCustodiansRequest**| Submit search query | |
| **sort** | [**string**] | Field to sort by (default: \&#39;score\&#39;) | (optional) defaults to undefined|
| **direction** | [**&#39;asc&#39; | &#39;desc&#39;**]**Array<&#39;asc&#39; &#124; &#39;desc&#39;>** | Sort direction (\&#39;asc\&#39; or \&#39;desc\&#39;, default: \&#39;desc\&#39;) | (optional) defaults to undefined|
| **perPage** | [**number**] | Number of results to return per page | (optional) defaults to undefined|


### Return type

**SearchDataCustodians200Response**

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

