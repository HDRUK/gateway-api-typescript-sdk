# UsersApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createUsers**](#createusers) | **POST** /api/v1/users | UserController@store|
|[**deleteUsers**](#deleteusers) | **DELETE** /api/v1/users/{id} | UserController@destroy|
|[**editUsers**](#editusers) | **PATCH** /api/v1/users/{id} | UserController@edit|
|[**fetchAllUsers**](#fetchallusers) | **GET** /api/v1/users | UserController@index|
|[**fetchUsers**](#fetchusers) | **GET** /api/v1/users/{id} | UserController@show|
|[**resendSecondaryVerificationEmail**](#resendsecondaryverificationemail) | **POST** /api/v1/users/{id}/resend-secondary-verification | Resend secondary email verification|
|[**updateUsers**](#updateusers) | **PUT** /api/v1/users/{id} | UserController@update|
|[**verifySecondaryEmail**](#verifysecondaryemail) | **GET** /api/v1/users/verify-secondary-email/{uuid} | Verify user\&#39;s secondary email using a UUID|

# **createUsers**
> CreateCategories200Response createUsers(createUsersRequest)

Create a new user

### Example

```typescript
import {
    UsersApi,
    Configuration,
    CreateUsersRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let createUsersRequest: CreateUsersRequest; //Pass user credentials

const { status, data } = await apiInstance.createUsers(
    createUsersRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createUsersRequest** | **CreateUsersRequest**| Pass user credentials | |


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
|**201** | Created |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteUsers**
> DeleteFederation200Response deleteUsers()

Delete User based in id

### Example

```typescript
import {
    UsersApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let id: number; //user id (default to undefined)

const { status, data } = await apiInstance.deleteUsers(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | user id | defaults to undefined|


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
|**401** | Unauthorized |  -  |
|**404** | Error response |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **editUsers**
> FetchUsers200Response editUsers(updateUsersRequest)

Edit user

### Example

```typescript
import {
    UsersApi,
    Configuration,
    UpdateUsersRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let id: number; //user id (default to undefined)
let updateUsersRequest: UpdateUsersRequest; //Pass user credentials

const { status, data } = await apiInstance.editUsers(
    id,
    updateUsersRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateUsersRequest** | **UpdateUsersRequest**| Pass user credentials | |
| **id** | [**number**] | user id | defaults to undefined|


### Return type

**FetchUsers200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**400** | Error |  -  |
|**401** | Unauthorized |  -  |
|**404** | Error response |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchAllUsers**
> FetchAllUsers200Response fetchAllUsers()

Get All Users

### Example

```typescript
import {
    UsersApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let filterNames: string; //Three or more characters to filter users names by (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllUsers(
    filterNames
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **filterNames** | [**string**] | Three or more characters to filter users names by | (optional) defaults to undefined|


### Return type

**FetchAllUsers200Response**

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

# **fetchUsers**
> FetchUsers200Response fetchUsers()

Get users by id

### Example

```typescript
import {
    UsersApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let id: number; //user id (default to undefined)

const { status, data } = await apiInstance.fetchUsers(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | user id | defaults to undefined|


### Return type

**FetchUsers200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**401** | Unauthorized |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **resendSecondaryVerificationEmail**
> ResendSecondaryVerificationEmail200Response resendSecondaryVerificationEmail()

Resends the verification email for the secondary email address. Old tokens are expired.

### Example

```typescript
import {
    UsersApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let id: number; //User ID (default to undefined)

const { status, data } = await apiInstance.resendSecondaryVerificationEmail(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | User ID | defaults to undefined|


### Return type

**ResendSecondaryVerificationEmail200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Verification email resent |  -  |
|**404** | User or secondary email not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateUsers**
> FetchUsers200Response updateUsers(updateUsersRequest)

Update user

### Example

```typescript
import {
    UsersApi,
    Configuration,
    UpdateUsersRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let id: number; //user id (default to undefined)
let updateUsersRequest: UpdateUsersRequest; //Pass user credentials

const { status, data } = await apiInstance.updateUsers(
    id,
    updateUsersRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateUsersRequest** | **UpdateUsersRequest**| Pass user credentials | |
| **id** | [**number**] | user id | defaults to undefined|


### Return type

**FetchUsers200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**400** | Error |  -  |
|**401** | Unauthorized |  -  |
|**404** | Error response |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

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

