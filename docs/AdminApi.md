# AdminApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**revokeAllTokensV2**](#revokealltokensv2) | **POST** /api/v2/admin/tokens/revoke_all | TokenRevocationController@revokeAll|

# **revokeAllTokensV2**
> RevokeAllTokensV2200Response revokeAllTokensV2()

Revoke every Gateway JWT issued up to now, including the caller\'s own. All users must sign in again.

### Example

```typescript
import {
    AdminApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new AdminApi(configuration);

const { status, data } = await apiInstance.revokeAllTokensV2();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**RevokeAllTokensV2200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

