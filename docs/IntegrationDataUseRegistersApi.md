# IntegrationDataUseRegistersApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createDurIntegrations**](#createdurintegrations) | **POST** /api/v1/integrations/dur | IntegrationDurController@store|
|[**deleteDurIntegrations**](#deletedurintegrations) | **DELETE** /api/v1/integrations/dur/{id} | Delete a dur|
|[**editDurIntegrations**](#editdurintegrations) | **PATCH** /api/v1/integrations/dur/{id} | Edit a dur|
|[**fetchAllDurIntegrations**](#fetchalldurintegrations) | **GET** /api/v1/integrations/dur | IntegrationDurController@index|
|[**fetchDurByIdIntegrations**](#fetchdurbyidintegrations) | **GET** /api/v1/integrations/dur/{id} | IntegrationDurController@show|
|[**updateDurIntegrations**](#updatedurintegrations) | **PUT** /api/v1/integrations/dur/{id} | Update a dur by id|

# **createDurIntegrations**
> CreateDarIntegration201Response createDurIntegrations(createDurIntegrationsRequest)

Create a new dur

### Example

```typescript
import {
    IntegrationDataUseRegistersApi,
    Configuration,
    CreateDurIntegrationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new IntegrationDataUseRegistersApi(configuration);

let createDurIntegrationsRequest: CreateDurIntegrationsRequest; //Pass user credentials

const { status, data } = await apiInstance.createDurIntegrations(
    createDurIntegrationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createDurIntegrationsRequest** | **CreateDurIntegrationsRequest**| Pass user credentials | |


### Return type

**CreateDarIntegration201Response**

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

# **deleteDurIntegrations**
> DeleteApplications200Response deleteDurIntegrations()

Delete a dur

### Example

```typescript
import {
    IntegrationDataUseRegistersApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new IntegrationDataUseRegistersApi(configuration);

let id: number; //dur id (default to undefined)

const { status, data } = await apiInstance.deleteDurIntegrations(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | dur id | defaults to undefined|


### Return type

**DeleteApplications200Response**

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

# **editDurIntegrations**
> UpdateDurIntegrations200Response editDurIntegrations(createDurIntegrationsRequest)

Edit a dur

### Example

```typescript
import {
    IntegrationDataUseRegistersApi,
    Configuration,
    CreateDurIntegrationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new IntegrationDataUseRegistersApi(configuration);

let id: number; //dur id (default to undefined)
let createDurIntegrationsRequest: CreateDurIntegrationsRequest; //Pass user credentials

const { status, data } = await apiInstance.editDurIntegrations(
    id,
    createDurIntegrationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createDurIntegrationsRequest** | **CreateDurIntegrationsRequest**| Pass user credentials | |
| **id** | [**number**] | dur id | defaults to undefined|


### Return type

**UpdateDurIntegrations200Response**

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

# **fetchAllDurIntegrations**
> FetchAllDurIntegrations200Response fetchAllDurIntegrations()

Returns a list of dur

### Example

```typescript
import {
    IntegrationDataUseRegistersApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new IntegrationDataUseRegistersApi(configuration);

let sort: ProjectTitleAscupdatedAtAsc; //Sort fields in the format field:direction, e.g., project_title:asc,updated_at:asc (optional) (default to undefined)
let perPage: number; //per page (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllDurIntegrations(
    sort,
    perPage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sort** | **ProjectTitleAscupdatedAtAsc** | Sort fields in the format field:direction, e.g., project_title:asc,updated_at:asc | (optional) defaults to undefined|
| **perPage** | [**number**] | per page | (optional) defaults to undefined|


### Return type

**FetchAllDurIntegrations200Response**

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

# **fetchDurByIdIntegrations**
> FetchDurByIdIntegrations200Response fetchDurByIdIntegrations()

Get dur by id

### Example

```typescript
import {
    IntegrationDataUseRegistersApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new IntegrationDataUseRegistersApi(configuration);

let id: number; //data use register id (default to undefined)

const { status, data } = await apiInstance.fetchDurByIdIntegrations(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | data use register id | defaults to undefined|


### Return type

**FetchDurByIdIntegrations200Response**

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

# **updateDurIntegrations**
> UpdateDurIntegrations200Response updateDurIntegrations(createDurIntegrationsRequest)

Update a dur

### Example

```typescript
import {
    IntegrationDataUseRegistersApi,
    Configuration,
    CreateDurIntegrationsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new IntegrationDataUseRegistersApi(configuration);

let id: number; //dur id (default to undefined)
let createDurIntegrationsRequest: CreateDurIntegrationsRequest; //Pass user credentials

const { status, data } = await apiInstance.updateDurIntegrations(
    id,
    createDurIntegrationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createDurIntegrationsRequest** | **CreateDurIntegrationsRequest**| Pass user credentials | |
| **id** | [**number**] | dur id | defaults to undefined|


### Return type

**UpdateDurIntegrations200Response**

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

