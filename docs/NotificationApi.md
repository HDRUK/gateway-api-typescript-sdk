# NotificationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createNotifications**](#createnotifications) | **POST** /api/v1/notifications | Notification@store|
|[**deleteNotifications**](#deletenotifications) | **DELETE** /api/v1/notifications/{id} | Notification@destroy|
|[**editNotifications**](#editnotifications) | **PATCH** /api/v1/notifications/{id} | Notification@edit|
|[**fetchAllNotifications**](#fetchallnotifications) | **GET** /api/v1/notifications | Notification@index|
|[**fetchNotifications**](#fetchnotifications) | **GET** /api/v1/notifications/{id} | Notification@show|
|[**updateNotifications**](#updatenotifications) | **PUT** /api/v1/notifications/{id} | Notification@update|

# **createNotifications**
> CreateCategories200Response createNotifications(createNotificationsRequest)

Creates a new notification

### Example

```typescript
import {
    NotificationApi,
    Configuration,
    CreateNotificationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new NotificationApi(configuration);

let createNotificationsRequest: CreateNotificationsRequest; //Notification definition

const { status, data } = await apiInstance.createNotifications(
    createNotificationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createNotificationsRequest** | **CreateNotificationsRequest**| Notification definition | |


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

# **deleteNotifications**
> DeleteAliases200Response deleteNotifications()

Delete a notification

### Example

```typescript
import {
    NotificationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new NotificationApi(configuration);

let id: number; //notification id (default to undefined)

const { status, data } = await apiInstance.deleteNotifications(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | notification id | defaults to undefined|


### Return type

**DeleteAliases200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**404** | Not found response |  -  |
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **editNotifications**
> UpdateNotifications200Response editNotifications(editNotificationsRequest)

Edit a notification

### Example

```typescript
import {
    NotificationApi,
    Configuration,
    EditNotificationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new NotificationApi(configuration);

let id: number; //notification id (default to undefined)
let editNotificationsRequest: EditNotificationsRequest; //Notification definition

const { status, data } = await apiInstance.editNotifications(
    id,
    editNotificationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editNotificationsRequest** | **EditNotificationsRequest**| Notification definition | |
| **id** | [**number**] | notification id | defaults to undefined|


### Return type

**UpdateNotifications200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**404** | Not found response |  -  |
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchAllNotifications**
> FetchAllNotifications200Response fetchAllNotifications()

Returns a list of notifications enabled on the system

### Example

```typescript
import {
    NotificationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new NotificationApi(configuration);

const { status, data } = await apiInstance.fetchAllNotifications();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**FetchAllNotifications200Response**

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

# **fetchNotifications**
> FetchNotifications200Response fetchNotifications()

Return a single notification

### Example

```typescript
import {
    NotificationApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new NotificationApi(configuration);

let id: number; //notification id (default to undefined)

const { status, data } = await apiInstance.fetchNotifications(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | notification id | defaults to undefined|


### Return type

**FetchNotifications200Response**

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

# **updateNotifications**
> UpdateNotifications200Response updateNotifications(createNotificationsRequest)

Update a notification

### Example

```typescript
import {
    NotificationApi,
    Configuration,
    CreateNotificationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new NotificationApi(configuration);

let id: number; //notification id (default to undefined)
let createNotificationsRequest: CreateNotificationsRequest; //Notification definition

const { status, data } = await apiInstance.updateNotifications(
    id,
    createNotificationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createNotificationsRequest** | **CreateNotificationsRequest**| Notification definition | |
| **id** | [**number**] | notification id | defaults to undefined|


### Return type

**UpdateNotifications200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**404** | Not found response |  -  |
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

