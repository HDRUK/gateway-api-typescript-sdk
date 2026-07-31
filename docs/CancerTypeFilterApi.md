# CancerTypeFilterApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getCancerTypeFilter**](#getcancertypefilter) | **GET** /api/v1/cancer-type-filters/{filter_id} | Get a single cancer type filter|
|[**getCancerTypeFilters**](#getcancertypefilters) | **GET** /api/v1/cancer-type-filters | Get all cancer type filters|

# **getCancerTypeFilter**
> GetCancerTypeFilter200Response getCancerTypeFilter()

Returns a single cancer type filter with its children by filter_id

### Example

```typescript
import {
    CancerTypeFilterApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CancerTypeFilterApi(configuration);

let filterId: string; //Filter ID (e.g., 0_0, 0_0_2_59) (default to undefined)

const { status, data } = await apiInstance.getCancerTypeFilter(
    filterId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **filterId** | [**string**] | Filter ID (e.g., 0_0, 0_0_2_59) | defaults to undefined|


### Return type

**GetCancerTypeFilter200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getCancerTypeFilters**
> GetCancerTypeFilters200Response getCancerTypeFilters()

Returns a hierarchical tree of cancer type filters

### Example

```typescript
import {
    CancerTypeFilterApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new CancerTypeFilterApi(configuration);

let parentId: number; //Filter by parent ID (optional) (default to undefined)
let level: number; //Filter by hierarchy level (optional) (default to undefined)

const { status, data } = await apiInstance.getCancerTypeFilters(
    parentId,
    level
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **parentId** | [**number**] | Filter by parent ID | (optional) defaults to undefined|
| **level** | [**number**] | Filter by hierarchy level | (optional) defaults to undefined|


### Return type

**GetCancerTypeFilters200Response**

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

