# UserOrganisationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**fetchUserOrganisations**](#fetchuserorganisations) | **GET** /api/v1/users/organisations | UserOrganisation@index|

# **fetchUserOrganisations**
> FetchUserOrganisations200Response fetchUserOrganisations()

Return a distinct list of all organisations which users belong to

### Example

```typescript
import {
    UserOrganisationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UserOrganisationApi(configuration);

const { status, data } = await apiInstance.fetchUserOrganisations();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**FetchUserOrganisations200Response**

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

