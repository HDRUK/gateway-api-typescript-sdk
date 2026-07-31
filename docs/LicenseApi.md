# LicenseApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createLicenses**](#createlicenses) | **POST** /api/v1/licenses | License@store|
|[**deleteLicenses**](#deletelicenses) | **DELETE** /api/v1/licenses/{id} | License@destroy|
|[**editLicenses**](#editlicenses) | **PATCH** /api/v1/licenses/{id} | License@edit|
|[**fetchAllLicenses**](#fetchalllicenses) | **GET** /api/v1/licenses | License@index|
|[**fetchLicenses**](#fetchlicenses) | **GET** /api/v1/licenses/{id} | License@show|
|[**updateLicenses**](#updatelicenses) | **PUT** /api/v1/licenses/{id} | License@update|

# **createLicenses**
> CreateCategories200Response createLicenses(createLicensesRequest)

Creates a new license

### Example

```typescript
import {
    LicenseApi,
    Configuration,
    CreateLicensesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new LicenseApi(configuration);

let createLicensesRequest: CreateLicensesRequest; //License definition

const { status, data } = await apiInstance.createLicenses(
    createLicensesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createLicensesRequest** | **CreateLicensesRequest**| License definition | |


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

# **deleteLicenses**
> DeleteAliases200Response deleteLicenses()

Delete a License

### Example

```typescript
import {
    LicenseApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new LicenseApi(configuration);

let id: number; //License id (default to undefined)

const { status, data } = await apiInstance.deleteLicenses(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | License id | defaults to undefined|


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

# **editLicenses**
> UpdateLicenses200Response editLicenses(createLicensesRequest)

Edit a tool license

### Example

```typescript
import {
    LicenseApi,
    Configuration,
    CreateLicensesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new LicenseApi(configuration);

let id: number; //license id (default to undefined)
let createLicensesRequest: CreateLicensesRequest; //Category definition

const { status, data } = await apiInstance.editLicenses(
    id,
    createLicensesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createLicensesRequest** | **CreateLicensesRequest**| Category definition | |
| **id** | [**number**] | license id | defaults to undefined|


### Return type

**UpdateLicenses200Response**

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

# **updateLicenses**
> UpdateLicenses200Response updateLicenses(createLicensesRequest)

Update a tool license

### Example

```typescript
import {
    LicenseApi,
    Configuration,
    CreateLicensesRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new LicenseApi(configuration);

let id: number; //license id (default to undefined)
let createLicensesRequest: CreateLicensesRequest; //Category definition

const { status, data } = await apiInstance.updateLicenses(
    id,
    createLicensesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createLicensesRequest** | **CreateLicensesRequest**| Category definition | |
| **id** | [**number**] | license id | defaults to undefined|


### Return type

**UpdateLicenses200Response**

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

