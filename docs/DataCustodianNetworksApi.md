# DataCustodianNetworksApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createDataCustodianNetwork**](#createdatacustodiannetwork) | **POST** /api/v2/data_custodian_networks | DataCustodianNetworks@store|
|[**deleteDataCustodianNetwork**](#deletedatacustodiannetwork) | **DELETE** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@destroy|
|[**editDataCustodianNetwork**](#editdatacustodiannetwork) | **PATCH** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@edit|
|[**fetchDataCustodianNetwork**](#fetchdatacustodiannetwork) | **GET** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@show|
|[**fetchDataCustodianNetworkCustodiansSummary**](#fetchdatacustodiannetworkcustodianssummary) | **GET** /api/v2/data_custodian_networks/{id}/custodians_summary | DataCustodianNetworks@showCustodiansSummary|
|[**fetchDataCustodianNetworkDatasetsSummary**](#fetchdatacustodiannetworkdatasetssummary) | **GET** /api/v2/data_custodian_networks/{id}/datasets_summary | DataCustodianNetworks@showDatasetsSummary|
|[**fetchDataCustodianNetworkEntitiesSummary**](#fetchdatacustodiannetworkentitiessummary) | **GET** /api/v2/data_custodian_networks/{id}/entities_summary | DataCustodianNetworks@showSummary|
|[**fetchDataCustodianNetworkInfo**](#fetchdatacustodiannetworkinfo) | **GET** /api/v2/data_custodian_networks/{id}/info | DataCustodianNetworks@showInfoSummary|
|[**fetchDataCustodianNetworks**](#fetchdatacustodiannetworks) | **GET** /api/v2/data_custodian_networks | DataCustodianNetworks@index|
|[**updateDataCustodianNetwork**](#updatedatacustodiannetwork) | **PUT** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@update|

# **createDataCustodianNetwork**
> CreateCategories200Response createDataCustodianNetwork(createDataProviderCollRequest)

Creates a new DataCustodianNetwork

### Example

```typescript
import {
    DataCustodianNetworksApi,
    Configuration,
    CreateDataProviderCollRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataCustodianNetworksApi(configuration);

let createDataProviderCollRequest: CreateDataProviderCollRequest; //DataCustodianNetwork definition

const { status, data } = await apiInstance.createDataCustodianNetwork(
    createDataProviderCollRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createDataProviderCollRequest** | **CreateDataProviderCollRequest**| DataCustodianNetwork definition | |


### Return type

**CreateCategories200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteDataCustodianNetwork**
> DeleteAliases200Response deleteDataCustodianNetwork()

Delete a DataCustodianNetwork

### Example

```typescript
import {
    DataCustodianNetworksApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataCustodianNetworksApi(configuration);

let id: number; //DataCustodianNetwork ID (default to undefined)

const { status, data } = await apiInstance.deleteDataCustodianNetwork(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DataCustodianNetwork ID | defaults to undefined|


### Return type

**DeleteAliases200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**404** | Not found response |  -  |
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **editDataCustodianNetwork**
> UpdateDataCustodianNetwork200Response editDataCustodianNetwork(editDataProviderCollRequest)

Edit a DataCustodianNetwork

### Example

```typescript
import {
    DataCustodianNetworksApi,
    Configuration,
    EditDataProviderCollRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataCustodianNetworksApi(configuration);

let id: number; //DataCustodianNetwork ID (default to undefined)
let editDataProviderCollRequest: EditDataProviderCollRequest; //DataCustodianNetwork definition

const { status, data } = await apiInstance.editDataCustodianNetwork(
    id,
    editDataProviderCollRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editDataProviderCollRequest** | **EditDataProviderCollRequest**| DataCustodianNetwork definition | |
| **id** | [**number**] | DataCustodianNetwork ID | defaults to undefined|


### Return type

**UpdateDataCustodianNetwork200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**404** | Not found response |  -  |
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

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

# **updateDataCustodianNetwork**
> UpdateDataCustodianNetwork200Response updateDataCustodianNetwork(updateDataProviderCollRequest)

Update a DataCustodianNetwork

### Example

```typescript
import {
    DataCustodianNetworksApi,
    Configuration,
    UpdateDataProviderCollRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataCustodianNetworksApi(configuration);

let id: number; //DataCustodianNetworks ID (default to undefined)
let updateDataProviderCollRequest: UpdateDataProviderCollRequest; //DataCustodianNetwork definition

const { status, data } = await apiInstance.updateDataCustodianNetwork(
    id,
    updateDataProviderCollRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateDataProviderCollRequest** | **UpdateDataProviderCollRequest**| DataCustodianNetwork definition | |
| **id** | [**number**] | DataCustodianNetworks ID | defaults to undefined|


### Return type

**UpdateDataCustodianNetwork200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**404** | Not found response |  -  |
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

