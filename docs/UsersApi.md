# UsersApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**verifySecondaryEmail**](#verifysecondaryemail) | **GET** /api/v1/users/verify-secondary-email/{uuid} | Verify user\&#39;s secondary email using a UUID|

# **verifySecondaryEmail**
> VerifySecondaryEmail200Response verifySecondaryEmail()

This endpoint verifies the secondary email for a user if the UUID is valid and not expired.

### Example

```typescript
import {
    UsersApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let uuid: string; //Verification UUID (default to undefined)

const { status, data } = await apiInstance.verifySecondaryEmail(
    uuid
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **uuid** | [**string**] | Verification UUID | defaults to undefined|


### Return type

**VerifySecondaryEmail200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Email verified successfully |  -  |
|**400** | Invalid or expired token |  -  |
|**404** | UUID not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

