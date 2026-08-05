# DataUseRegistersApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createDur**](#createdur) | **POST** /api/v1/dur | DurController@store|
|[**createDurByTeamV2**](#createdurbyteamv2) | **POST** /api/v2/teams/{teamId}/dur | TeamDurController@store|
|[**deleteDur**](#deletedur) | **DELETE** /api/v1/dur/{id} | Delete a dur|
|[**deleteDursV2ByTeamId**](#deletedursv2byteamid) | **DELETE** /api/v2/teams/{teamId}/dur/{id} | TeamDurController@destroy|
|[**editDur**](#editdur) | **PATCH** /api/v1/dur/{id} | Edit a dur|
|[**editDursV2ByTeamId**](#editdursv2byteamid) | **PATCH** /api/v2/teams/{teamId}/dur/{id} | TeamDurController@edit|
|[**exportDurTemplate**](#exportdurtemplate) | **GET** /api/v1/dur/template | DurController@exportTemplate|
|[**exportDurTemplateV2**](#exportdurtemplatev2) | **GET** /api/v2/dur/template | DurController@exportTemplate|
|[**exportDurV2**](#exportdurv2) | **GET** /api/v2/dur/export | DurController@export|
|[**fetchAllDur**](#fetchalldur) | **GET** /api/v1/dur | DurController@index|
|[**fetchAllDurV2**](#fetchalldurv2) | **GET** /api/v2/dur | DurController@indexActive|
|[**fetchDurById**](#fetchdurbyid) | **GET** /api/v1/dur/{id} | DurController@show|
|[**fetchDurByIdV2**](#fetchdurbyidv2) | **GET** /api/v2/dur/{id} | DurController@showActive|
|[**updateDur**](#updatedur) | **PUT** /api/v1/dur/{id} | Update a dur by id|
|[**updateDurV2ByTeamId**](#updatedurv2byteamid) | **PUT** /api/v2/teams/{teamId}/dur/{id} | TeamDurController@update|
|[**uploadDur**](#uploaddur) | **POST** /api/v1/dur/upload | DurController@upload|

# **createDur**
> CreateDarIntegration201Response createDur(createDurRequest)

Create a new dur

### Example

```typescript
import {
    DataUseRegistersApi,
    Configuration,
    CreateDurRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataUseRegistersApi(configuration);

let createDurRequest: CreateDurRequest; //Pass user credentials

const { status, data } = await apiInstance.createDur(
    createDurRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createDurRequest** | **CreateDurRequest**| Pass user credentials | |


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

# **createDurByTeamV2**
> CreateDarIntegration201Response createDurByTeamV2(createDurRequest)

Create a new dur by team v2

### Example

```typescript
import {
    DataUseRegistersApi,
    Configuration,
    CreateDurRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataUseRegistersApi(configuration);

let teamId: number; //team id (default to undefined)
let createDurRequest: CreateDurRequest; //Pass user credentials

const { status, data } = await apiInstance.createDurByTeamV2(
    teamId,
    createDurRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createDurRequest** | **CreateDurRequest**| Pass user credentials | |
| **teamId** | [**number**] | team id | defaults to undefined|


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

# **deleteDur**
> DeleteApplications200Response deleteDur()

Delete a dur

### Example

```typescript
import {
    DataUseRegistersApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataUseRegistersApi(configuration);

let id: number; //dur id (default to undefined)

const { status, data } = await apiInstance.deleteDur(
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

# **deleteDursV2ByTeamId**
> DeleteApplications200Response deleteDursV2ByTeamId()

Delete a dur by team and id v2

### Example

```typescript
import {
    DataUseRegistersApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataUseRegistersApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //dur id (default to undefined)

const { status, data } = await apiInstance.deleteDursV2ByTeamId(
    teamId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|
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

# **editDur**
> UpdateDur200Response editDur(createDurRequest)

Edit a dur

### Example

```typescript
import {
    DataUseRegistersApi,
    Configuration,
    CreateDurRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataUseRegistersApi(configuration);

let id: number; //dur id (default to undefined)
let createDurRequest: CreateDurRequest; //Pass user credentials
let unarchive: string; //Unarchive a dur (optional) (default to undefined)

const { status, data } = await apiInstance.editDur(
    id,
    createDurRequest,
    unarchive
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createDurRequest** | **CreateDurRequest**| Pass user credentials | |
| **id** | [**number**] | dur id | defaults to undefined|
| **unarchive** | [**string**] | Unarchive a dur | (optional) defaults to undefined|


### Return type

**UpdateDur200Response**

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

# **editDursV2ByTeamId**
> UpdateDur200Response editDursV2ByTeamId(createDurRequest)

Edit a dur by team v2

### Example

```typescript
import {
    DataUseRegistersApi,
    Configuration,
    CreateDurRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataUseRegistersApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //dur id (default to undefined)
let createDurRequest: CreateDurRequest; //Pass user credentials

const { status, data } = await apiInstance.editDursV2ByTeamId(
    teamId,
    id,
    createDurRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createDurRequest** | **CreateDurRequest**| Pass user credentials | |
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | dur id | defaults to undefined|


### Return type

**UpdateDur200Response**

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

# **exportDurTemplate**
> any exportDurTemplate()

Export Dur upload template

### Example

```typescript
import {
    DataUseRegistersApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataUseRegistersApi(configuration);

const { status, data } = await apiInstance.exportDurTemplate();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**any**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/csv, application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | File download |  -  |
|**401** | Unauthorized |  -  |
|**404** | File Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **exportDurTemplateV2**
> any exportDurTemplateV2()

Export Dur upload template

### Example

```typescript
import {
    DataUseRegistersApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataUseRegistersApi(configuration);

const { status, data } = await apiInstance.exportDurTemplateV2();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**any**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/csv, application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | File download |  -  |
|**401** | Unauthorized |  -  |
|**404** | File Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **exportDurV2**
> string exportDurV2()

Export CSV of one or more DURs

### Example

```typescript
import {
    DataUseRegistersApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataUseRegistersApi(configuration);

let id: number; //dur id (optional) (default to undefined)

const { status, data } = await apiInstance.exportDurV2(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | dur id | (optional) defaults to undefined|


### Return type

**string**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/csv, application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | CSV file |  -  |
|**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchAllDur**
> FetchAllDur200Response fetchAllDur()

Returns a list of dur

### Example

```typescript
import {
    DataUseRegistersApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataUseRegistersApi(configuration);

let sort: ProjectTitleAscupdatedAtAsc; //Sort fields in the format field:direction, e.g., project_title:asc,updated_at:asc (optional) (default to undefined)
let projectTitle: string; //Filter tools by project title (optional) (default to undefined)
let perPage: number; //per page (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllDur(
    sort,
    projectTitle,
    perPage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sort** | **ProjectTitleAscupdatedAtAsc** | Sort fields in the format field:direction, e.g., project_title:asc,updated_at:asc | (optional) defaults to undefined|
| **projectTitle** | [**string**] | Filter tools by project title | (optional) defaults to undefined|
| **perPage** | [**number**] | per page | (optional) defaults to undefined|


### Return type

**FetchAllDur200Response**

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

# **fetchAllDurV2**
> FetchAllDurV2200Response fetchAllDurV2()

Returns a list of active dur

### Example

```typescript
import {
    DataUseRegistersApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataUseRegistersApi(configuration);

let sort: ProjectTitleAscupdatedAtAsc; //Sort fields in the format field:direction, e.g., project_title:asc,updated_at:asc (optional) (default to undefined)
let projectTitle: string; //Filter tools by project title (optional) (default to undefined)
let perPage: number; //per page (optional) (default to undefined)
let withRelated: boolean; //Show related entities (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllDurV2(
    sort,
    projectTitle,
    perPage,
    withRelated
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sort** | **ProjectTitleAscupdatedAtAsc** | Sort fields in the format field:direction, e.g., project_title:asc,updated_at:asc | (optional) defaults to undefined|
| **projectTitle** | [**string**] | Filter tools by project title | (optional) defaults to undefined|
| **perPage** | [**number**] | per page | (optional) defaults to undefined|
| **withRelated** | [**boolean**] | Show related entities | (optional) defaults to undefined|


### Return type

**FetchAllDurV2200Response**

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

# **fetchDurById**
> FetchDurById200Response fetchDurById()

Get dur by id

### Example

```typescript
import {
    DataUseRegistersApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataUseRegistersApi(configuration);

let id: number; //data use register id (default to undefined)

const { status, data } = await apiInstance.fetchDurById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | data use register id | defaults to undefined|


### Return type

**FetchDurById200Response**

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

# **fetchDurByIdV2**
> UpdateDur200Response fetchDurByIdV2()

Get dur by id

### Example

```typescript
import {
    DataUseRegistersApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataUseRegistersApi(configuration);

let id: number; //data use register id (default to undefined)

const { status, data } = await apiInstance.fetchDurByIdV2(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | data use register id | defaults to undefined|


### Return type

**UpdateDur200Response**

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

# **updateDur**
> UpdateDur200Response updateDur(createDurRequest)

Update a dur

### Example

```typescript
import {
    DataUseRegistersApi,
    Configuration,
    CreateDurRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataUseRegistersApi(configuration);

let id: number; //dur id (default to undefined)
let createDurRequest: CreateDurRequest; //Pass user credentials

const { status, data } = await apiInstance.updateDur(
    id,
    createDurRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createDurRequest** | **CreateDurRequest**| Pass user credentials | |
| **id** | [**number**] | dur id | defaults to undefined|


### Return type

**UpdateDur200Response**

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

# **updateDurV2ByTeamId**
> UpdateDur200Response updateDurV2ByTeamId(createDurRequest)

Update a dur by team and id v2

### Example

```typescript
import {
    DataUseRegistersApi,
    Configuration,
    CreateDurRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataUseRegistersApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //dur id (default to undefined)
let createDurRequest: CreateDurRequest; //Pass user credentials

const { status, data } = await apiInstance.updateDurV2ByTeamId(
    teamId,
    id,
    createDurRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createDurRequest** | **CreateDurRequest**| Pass user credentials | |
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | dur id | defaults to undefined|


### Return type

**UpdateDur200Response**

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

# **uploadDur**
> CreateDarIntegration201Response uploadDur(uploadDurRequest)

Create a new dur with upload data

### Example

```typescript
import {
    DataUseRegistersApi,
    Configuration,
    UploadDurRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataUseRegistersApi(configuration);

let uploadDurRequest: UploadDurRequest; //Pass user credentials

const { status, data } = await apiInstance.uploadDur(
    uploadDurRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **uploadDurRequest** | **UploadDurRequest**| Pass user credentials | |


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

