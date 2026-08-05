# DataCustodianNetworksApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**fetchDataCustodianNetwork**](#fetchdatacustodiannetwork) | **GET** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@show|
|[**fetchDataCustodianNetworkCustodiansSummary**](#fetchdatacustodiannetworkcustodianssummary) | **GET** /api/v2/data_custodian_networks/{id}/custodians_summary | DataCustodianNetworks@showCustodiansSummary|
|[**fetchDataCustodianNetworkDatasetsSummary**](#fetchdatacustodiannetworkdatasetssummary) | **GET** /api/v2/data_custodian_networks/{id}/datasets_summary | DataCustodianNetworks@showDatasetsSummary|
|[**fetchDataCustodianNetworkEntitiesSummary**](#fetchdatacustodiannetworkentitiessummary) | **GET** /api/v2/data_custodian_networks/{id}/entities_summary | DataCustodianNetworks@showSummary|
|[**fetchDataCustodianNetworkInfo**](#fetchdatacustodiannetworkinfo) | **GET** /api/v2/data_custodian_networks/{id}/info | DataCustodianNetworks@showInfoSummary|
|[**fetchDataCustodianNetworks**](#fetchdatacustodiannetworks) | **GET** /api/v2/data_custodian_networks | DataCustodianNetworks@index|

# **fetchDataCustodianNetwork**
> FetchDataCustodianNetwork200Response fetchDataCustodianNetwork()

Return a single DataCustodianNetwork

### Example

```typescript
import {
    DataCustodianNetworksApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataCustodianNetworksApi(configuration);

let id: number; //DataCustodianNetwork ID (default to undefined)

const { status, data } = await apiInstance.fetchDataCustodianNetwork(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DataCustodianNetwork ID | defaults to undefined|


### Return type

**FetchDataCustodianNetwork200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDataCustodianNetworkCustodiansSummary**
> FetchDataCustodianNetworkCustodiansSummary200Response fetchDataCustodianNetworkCustodiansSummary()

Return a single DataCustodianNetwork - custodians summary

### Example

```typescript
import {
    DataCustodianNetworksApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataCustodianNetworksApi(configuration);

let id: number; //DataCustodianNetwork ID - summary (default to undefined)

const { status, data } = await apiInstance.fetchDataCustodianNetworkCustodiansSummary(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DataCustodianNetwork ID - summary | defaults to undefined|


### Return type

**FetchDataCustodianNetworkCustodiansSummary200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDataCustodianNetworkDatasetsSummary**
> FetchDataCustodianNetworkDatasetsSummary200Response fetchDataCustodianNetworkDatasetsSummary()

Return a single DataCustodianNetwork - summary of datasets

### Example

```typescript
import {
    DataCustodianNetworksApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataCustodianNetworksApi(configuration);

let id: number; //DataCustodianNetwork ID - summary (default to undefined)

const { status, data } = await apiInstance.fetchDataCustodianNetworkDatasetsSummary(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DataCustodianNetwork ID - summary | defaults to undefined|


### Return type

**FetchDataCustodianNetworkDatasetsSummary200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDataCustodianNetworkEntitiesSummary**
> FetchDataCustodianNetworkEntitiesSummary200Response fetchDataCustodianNetworkEntitiesSummary()

Return a single DataCustodianNetwork - summary of entities

### Example

```typescript
import {
    DataCustodianNetworksApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataCustodianNetworksApi(configuration);

let id: number; //DataCustodianNetwork ID - summary (default to undefined)

const { status, data } = await apiInstance.fetchDataCustodianNetworkEntitiesSummary(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DataCustodianNetwork ID - summary | defaults to undefined|


### Return type

**FetchDataCustodianNetworkEntitiesSummary200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDataCustodianNetworkInfo**
> FetchDataCustodianNetworkInfo200Response fetchDataCustodianNetworkInfo()

Return a single DataCustodianNetwork - basic information

### Example

```typescript
import {
    DataCustodianNetworksApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataCustodianNetworksApi(configuration);

let id: number; //DataCustodianNetwork ID - summary (default to undefined)

const { status, data } = await apiInstance.fetchDataCustodianNetworkInfo(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DataCustodianNetwork ID - summary | defaults to undefined|


### Return type

**FetchDataCustodianNetworkInfo200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDataCustodianNetworks**
> FetchDataCustodianNetworks200Response fetchDataCustodianNetworks()

Returns a list of DataCustodianNetworks enabled on the system

### Example

```typescript
import {
    DataCustodianNetworksApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataCustodianNetworksApi(configuration);

let perPage: number; //per page (optional) (default to undefined)

const { status, data } = await apiInstance.fetchDataCustodianNetworks(
    perPage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **perPage** | [**number**] | per page | (optional) defaults to undefined|


### Return type

**FetchDataCustodianNetworks200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

