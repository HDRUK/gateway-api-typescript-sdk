# SearchDataCustodianNetworksApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**searchDataCustodianNetworks**](#searchdatacustodiannetworks) | **POST** /api/v1/search/data_custodian_networks | Search@data_custodian_networks|

# **searchDataCustodianNetworks**
> SearchDataCustodianNetworks200Response searchDataCustodianNetworks(searchDataCustodianNetworksRequest)

Returns gateway data custodian networks related to the provided query term(s)

### Example

```typescript
import {
    SearchDataCustodianNetworksApi,
    Configuration,
    SearchDataCustodianNetworksRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new SearchDataCustodianNetworksApi(configuration);

let searchDataCustodianNetworksRequest: SearchDataCustodianNetworksRequest; //Submit search query
let sort: string; //Field to sort by (default: \'score\') (optional) (default to undefined)
let direction: 'asc' | 'desc'; //Sort direction (\'asc\' or \'desc\', default: \'desc\') (optional) (default to undefined)

const { status, data } = await apiInstance.searchDataCustodianNetworks(
    searchDataCustodianNetworksRequest,
    sort,
    direction
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **searchDataCustodianNetworksRequest** | **SearchDataCustodianNetworksRequest**| Submit search query | |
| **sort** | [**string**] | Field to sort by (default: \&#39;score\&#39;) | (optional) defaults to undefined|
| **direction** | [**&#39;asc&#39; | &#39;desc&#39;**]**Array<&#39;asc&#39; &#124; &#39;desc&#39;>** | Sort direction (\&#39;asc\&#39; or \&#39;desc\&#39;, default: \&#39;desc\&#39;) | (optional) defaults to undefined|


### Return type

**SearchDataCustodianNetworks200Response**

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

