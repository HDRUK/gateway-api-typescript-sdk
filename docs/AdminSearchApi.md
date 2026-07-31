# AdminSearchApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAdminSearchReindex**](#createadminsearchreindex) | **POST** /api/v1/admin/search/reindex | Queue a drop+recreate+import of a search entity\&#39;s Typesense collection|
|[**fetchAdminSearchStatus**](#fetchadminsearchstatus) | **GET** /api/v1/admin/search/status | Get Typesense collection status for every onboarded search entity|
|[**updateAdminSearchFeature**](#updateadminsearchfeature) | **POST** /api/v1/admin/search/feature | Activate or deactivate a search-related Pennant feature flag|

# **createAdminSearchReindex**
> createAdminSearchReindex(createAdminSearchReindexRequest)


### Example

```typescript
import {
    AdminSearchApi,
    Configuration,
    CreateAdminSearchReindexRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new AdminSearchApi(configuration);

let createAdminSearchReindexRequest: CreateAdminSearchReindexRequest; //

const { status, data } = await apiInstance.createAdminSearchReindex(
    createAdminSearchReindexRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createAdminSearchReindexRequest** | **CreateAdminSearchReindexRequest**|  | |


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**202** | Reindex queued |  -  |
|**422** | Unknown entity |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchAdminSearchStatus**
> fetchAdminSearchStatus()


### Example

```typescript
import {
    AdminSearchApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new AdminSearchApi(configuration);

const { status, data } = await apiInstance.fetchAdminSearchStatus();
```

### Parameters
This endpoint does not have any parameters.


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

# **updateAdminSearchFeature**
> updateAdminSearchFeature(updateAdminSearchFeatureRequest)


### Example

```typescript
import {
    AdminSearchApi,
    Configuration,
    UpdateAdminSearchFeatureRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new AdminSearchApi(configuration);

let updateAdminSearchFeatureRequest: UpdateAdminSearchFeatureRequest; //

const { status, data } = await apiInstance.updateAdminSearchFeature(
    updateAdminSearchFeatureRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateAdminSearchFeatureRequest** | **UpdateAdminSearchFeatureRequest**|  | |


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**422** | Unknown feature |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

