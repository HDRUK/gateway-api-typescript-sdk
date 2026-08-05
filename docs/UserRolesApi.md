# UserRolesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createUserHasRoles**](#createuserhasroles) | **POST** /api/v1/users/{userId}/roles | UserRoleController@store|
|[**deleteUserHasRoles**](#deleteuserhasroles) | **DELETE** /api/v1/users/{userId}/roles | UserRoleController@destroy|
|[**updateUserHasRoles**](#updateuserhasroles) | **PATCH** /api/v1/users/{userId}/roles | UserRoleController@edit|

# **createUserHasRoles**
> DeleteApplications200Response createUserHasRoles(createUserHasRolesRequest)

Create user has roles

### Example

```typescript
import {
    UserRolesApi,
    Configuration,
    CreateUserHasRolesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UserRolesApi(configuration);

let userId: number; //user id (default to undefined)
let createUserHasRolesRequest: CreateUserHasRolesRequest; //Pass user credentials

const { status, data } = await apiInstance.createUserHasRoles(
    userId,
    createUserHasRolesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createUserHasRolesRequest** | **CreateUserHasRolesRequest**| Pass user credentials | |
| **userId** | [**number**] | user id | defaults to undefined|


### Return type

**DeleteApplications200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Created |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteUserHasRoles**
> DeleteFederation200Response deleteUserHasRoles()

Delete user - roles

### Example

```typescript
import {
    UserRolesApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UserRolesApi(configuration);

let userId: number; //user id (default to undefined)

const { status, data } = await apiInstance.deleteUserHasRoles(
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | user id | defaults to undefined|


### Return type

**DeleteFederation200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**404** | Error response |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateUserHasRoles**
> DeleteApplications200Response updateUserHasRoles(updateUserHasRolesRequest)

Update user has roles

### Example

```typescript
import {
    UserRolesApi,
    Configuration,
    UpdateUserHasRolesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UserRolesApi(configuration);

let userId: number; //user id (default to undefined)
let updateUserHasRolesRequest: UpdateUserHasRolesRequest; //Pass user credentials

const { status, data } = await apiInstance.updateUserHasRoles(
    userId,
    updateUserHasRolesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateUserHasRolesRequest** | **UpdateUserHasRolesRequest**| Pass user credentials | |
| **userId** | [**number**] | user id | defaults to undefined|


### Return type

**DeleteApplications200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Created |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

