# AuthenticationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**authentication**](#authentication) | **POST** /api/v1/auth | AuthController@checkAuthorization|
|[**login**](#login) | **POST** /api/v1/auth/login | AuthController@login|
|[**refreshToken**](#refreshtoken) | **POST** /api/v1/refresh_token | AuthController@refreshToken|
|[**register**](#register) | **POST** /api/v1/auth/register | AuthController@register|

# **authentication**
> Authentication200Response authentication(authenticationRequest)

Generate Jwt based on email and password

### Example

```typescript
import {
    AuthenticationApi,
    Configuration,
    AuthenticationRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new AuthenticationApi(configuration);

let authenticationRequest: AuthenticationRequest; //Pass user credentials

const { status, data } = await apiInstance.authentication(
    authenticationRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **authenticationRequest** | **AuthenticationRequest**| Pass user credentials | |


### Return type

**Authentication200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**401** | Missing Property |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **login**
> Register200Response login(loginRequest)

Login with email and password

### Example

```typescript
import {
    AuthenticationApi,
    Configuration,
    LoginRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new AuthenticationApi(configuration);

let loginRequest: LoginRequest; //Pass user credentials

const { status, data } = await apiInstance.login(
    loginRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **loginRequest** | **LoginRequest**| Pass user credentials | |


### Return type

**Register200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**400** | Validation error |  -  |
|**401** | Invalid credentials |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **refreshToken**
> Authentication200Response refreshToken()

Regenerate jwt token

### Example

```typescript
import {
    AuthenticationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new AuthenticationApi(configuration);

const { status, data } = await apiInstance.refreshToken();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Authentication200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**401** | Missing Property |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **register**
> Register200Response register(registerRequest)

Register a new user with email and password

### Example

```typescript
import {
    AuthenticationApi,
    Configuration,
    RegisterRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new AuthenticationApi(configuration);

let registerRequest: RegisterRequest; //Pass user registration data

const { status, data } = await apiInstance.register(
    registerRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registerRequest** | **RegisterRequest**| Pass user registration data | |


### Return type

**Register200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**400** | Validation error |  -  |
|**409** | Email already exists |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

