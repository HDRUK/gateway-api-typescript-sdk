# LicenseApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**fetchAllLicenses**](#fetchalllicenses) | **GET** /api/v1/licenses | License@index|
|[**fetchLicenses**](#fetchlicenses) | **GET** /api/v1/licenses/{id} | License@show|

# **fetchAllLicenses**
> FetchAllLicenses200Response fetchAllLicenses()

Returns a list of licenses available

### Example

```typescript
import {
    LicenseApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new LicenseApi(configuration);

const { status, data } = await apiInstance.fetchAllLicenses();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**FetchAllLicenses200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchLicenses**
> FetchLicenses200Response fetchLicenses()

Return a single license

### Example

```typescript
import {
    LicenseApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new LicenseApi(configuration);

let id: number; //License ID (default to undefined)

const { status, data } = await apiInstance.fetchLicenses(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | License ID | defaults to undefined|


### Return type

**FetchLicenses200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

