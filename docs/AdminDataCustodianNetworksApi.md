# AdminDataCustodianNetworksApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**fetchAdminDataCustodianNetworks**](#fetchadmindatacustodiannetworks) | **GET** /api/v2/admin/data_custodian_networks | DataCustodianNetworks@adminIndex|

# **fetchAdminDataCustodianNetworks**
> fetchAdminDataCustodianNetworks()

Superadmin-only listing used by the network management admin screen — unlike index(), this is not filtered to enabled=1, so disabled networks remain visible/manageable.

### Example

```typescript
import {
    AdminDataCustodianNetworksApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new AdminDataCustodianNetworksApi(configuration);

let perPage: number; //per page (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAdminDataCustodianNetworks(
    perPage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **perPage** | [**number**] | per page | (optional) defaults to undefined|


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

