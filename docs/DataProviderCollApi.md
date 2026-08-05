# DataProviderCollApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**fetchDataProviderColl**](#fetchdataprovidercoll) | **GET** /api/v1/data_provider_colls/{id} | DataProviderColl@show|
|[**fetchDataProviderCollSummary**](#fetchdataprovidercollsummary) | **GET** /api/v1/data_provider_colls/{id}/summary | DataProviderColl@showSummary|
|[**fetchDataProviderColls**](#fetchdataprovidercolls) | **GET** /api/v1/data_provider_colls | DataProviderColl@index|

# **fetchDataProviderColl**
> FetchDataProviderColl200Response fetchDataProviderColl()

Return a single DataProviderColl

### Example

```typescript
import {
    DataProviderCollApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataProviderCollApi(configuration);

let id: number; //DataProviderColl ID (default to undefined)

const { status, data } = await apiInstance.fetchDataProviderColl(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DataProviderColl ID | defaults to undefined|


### Return type

**FetchDataProviderColl200Response**

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

# **fetchDataProviderCollSummary**
> FetchDataProviderCollSummary200Response fetchDataProviderCollSummary()

Return a single DataProviderColl - summary

### Example

```typescript
import {
    DataProviderCollApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataProviderCollApi(configuration);

let id: number; //DataProviderColl ID - summary (default to undefined)

const { status, data } = await apiInstance.fetchDataProviderCollSummary(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | DataProviderColl ID - summary | defaults to undefined|


### Return type

**FetchDataProviderCollSummary200Response**

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

# **fetchDataProviderColls**
> FetchDataProviderColls200Response fetchDataProviderColls()

Returns a list of DataProviderColls enabled on the system

### Example

```typescript
import {
    DataProviderCollApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataProviderCollApi(configuration);

let perPage: number; //per page (optional) (default to undefined)

const { status, data } = await apiInstance.fetchDataProviderColls(
    perPage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **perPage** | [**number**] | per page | (optional) defaults to undefined|


### Return type

**FetchDataProviderColls200Response**

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

