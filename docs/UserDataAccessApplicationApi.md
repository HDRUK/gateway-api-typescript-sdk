# UserDataAccessApplicationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**countAllUserDarApplications**](#countalluserdarapplications) | **GET** /api/v1/users/{userId}/dar/applications/count | UserDataAccessApplicationController@allCounts|
|[**countUserDarApplicationsByField**](#countuserdarapplicationsbyfield) | **GET** /api/v1/users/{userId}/dar/applications/count/{field} | UserDataAccessApplicationController@count|
|[**createUserDarApplicationAnswers**](#createuserdarapplicationanswers) | **PUT** /api/v1/users/{userId}/dar/applications/{id}/answers | UserDataAccessApplication@storeAnswers|
|[**fetchUserDarApplicationAnswers**](#fetchuserdarapplicationanswers) | **GET** /api/v1/users/{userId}/dar/applications/{id}/answers | UserDataAccessApplicationController@showAnswers|
|[**fetchUserDarApplicationDetails**](#fetchuserdarapplicationdetails) | **GET** /api/v1/users/{userId}/dar/applications/{id} | UserDataAccessApplicationController@show|
|[**fetchUserDarApplicationHeader**](#fetchuserdarapplicationheader) | **GET** /api/v1/users/{userId}/dar/applications/{id}/showHeader | UserDataAccessApplicationController@showHeader|
|[**fetchUserDarApplications**](#fetchuserdarapplications) | **GET** /api/v1/users/{userId}/dar/applications | UserDataAccessApplicationController@index|

# **countAllUserDarApplications**
> CountUniqueFieldsCollections200Response countAllUserDarApplications()

Get Counts for all status fields in the model

### Example

```typescript
import {
    UserDataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UserDataAccessApplicationApi(configuration);

let userId: number; //User id (default to undefined)

const { status, data } = await apiInstance.countAllUserDarApplications(
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | User id | defaults to undefined|


### Return type

**CountUniqueFieldsCollections200Response**

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

# **countUserDarApplicationsByField**
> CountUniqueFieldsCollections200Response countUserDarApplicationsByField()

Get Counts for distinct entries of a field in the model

### Example

```typescript
import {
    UserDataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UserDataAccessApplicationApi(configuration);

let userId: number; //User id (default to undefined)
let field: string; //name of the field to perform a count on (default to undefined)

const { status, data } = await apiInstance.countUserDarApplicationsByField(
    userId,
    field
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | User id | defaults to undefined|
| **field** | [**string**] | name of the field to perform a count on | defaults to undefined|


### Return type

**CountUniqueFieldsCollections200Response**

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

# **createUserDarApplicationAnswers**
> CreateCategories200Response createUserDarApplicationAnswers(createUserDarApplicationAnswersRequest)

Add answers to the user\'s DAR application

### Example

```typescript
import {
    UserDataAccessApplicationApi,
    Configuration,
    CreateUserDarApplicationAnswersRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UserDataAccessApplicationApi(configuration);

let userId: number; //User id (default to undefined)
let id: number; //DAR application id (default to undefined)
let createUserDarApplicationAnswersRequest: CreateUserDarApplicationAnswersRequest; //UserDataAccessApplication definition

const { status, data } = await apiInstance.createUserDarApplicationAnswers(
    userId,
    id,
    createUserDarApplicationAnswersRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createUserDarApplicationAnswersRequest** | **CreateUserDarApplicationAnswersRequest**| UserDataAccessApplication definition | |
| **userId** | [**number**] | User id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|


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
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchUserDarApplicationAnswers**
> FetchTeamDarApplicationAnswers200Response fetchUserDarApplicationAnswers()

Return answers from the user\'s DAR application

### Example

```typescript
import {
    UserDataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UserDataAccessApplicationApi(configuration);

let userId: number; //User id (default to undefined)
let id: number; //DAR application id (default to undefined)

const { status, data } = await apiInstance.fetchUserDarApplicationAnswers(
    userId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | User id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|


### Return type

**FetchTeamDarApplicationAnswers200Response**

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

# **fetchUserDarApplicationDetails**
> FetchTeamDarApplication200Response fetchUserDarApplicationDetails()

Return a DAR application belonging to the user

### Example

```typescript
import {
    UserDataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UserDataAccessApplicationApi(configuration);

let userId: number; //User id (default to undefined)
let id: number; //DAR application id (default to undefined)

const { status, data } = await apiInstance.fetchUserDarApplicationDetails(
    userId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | User id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|


### Return type

**FetchTeamDarApplication200Response**

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

# **fetchUserDarApplicationHeader**
> FetchTeamDarApplication200Response fetchUserDarApplicationHeader()

Get header information about a specific DAR

### Example

```typescript
import {
    UserDataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UserDataAccessApplicationApi(configuration);

let userId: number; //User id (default to undefined)
let id: number; //DAR application id (default to undefined)

const { status, data } = await apiInstance.fetchUserDarApplicationHeader(
    userId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | User id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|


### Return type

**FetchTeamDarApplication200Response**

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

# **fetchUserDarApplications**
> FetchTeamDarApplications200Response fetchUserDarApplications()

List of dar applications belonging to a user

### Example

```typescript
import {
    UserDataAccessApplicationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new UserDataAccessApplicationApi(configuration);

let userId: number; //User id (default to undefined)

const { status, data } = await apiInstance.fetchUserDarApplications(
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | User id | defaults to undefined|


### Return type

**FetchTeamDarApplications200Response**

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

