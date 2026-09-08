# DatasetsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**countUniqueFields**](#countuniquefields) | **GET** /api/v1/datasets/count/{field} | DatasetController@count|
|[**createDatasets**](#createdatasets) | **POST** /api/v1/datasets | DatasetController@store|
|[**createDatasetsV2**](#createdatasetsv2) | **POST** /api/v2/datasets | DatasetController@store|
|[**createTeamDatasetsV2**](#createteamdatasetsv2) | **POST** /api/v2/teams/{teamId}/datasets | TeamDatasetController@store|
|[**deleteDatasets**](#deletedatasets) | **DELETE** /api/v1/datasets/{id} | DatasetController@destroy|
|[**deleteDatasetsV2**](#deletedatasetsv2) | **DELETE** /api/v2/datasets/{id} | Delete a dataset|
|[**deleteTeamDatasetsV2**](#deleteteamdatasetsv2) | **DELETE** /api/v2/teams/{teamId}/datasets/{id} | TeamDatasetController@destroy|
|[**exportDatasetMetadata**](#exportdatasetmetadata) | **GET** /api/v1/datasets/export_metadata/{id} | DatasetController@exportMetadata|
|[**exportDatasets**](#exportdatasets) | **GET** /api/v1/datasets/export | DatasetController@export|
|[**exportDur**](#exportdur) | **GET** /api/v1/dur/export | DurController@export|
|[**exportMockDataset**](#exportmockdataset) | **GET** /api/v1/datasets/export/mock | DatasetController@exportMock|
|[**exportMockDatasetV2**](#exportmockdatasetv2) | **GET** /api/v2/datasets/export/mock | DatasetController@exportMock|
|[**fetchAllDatasets**](#fetchalldatasets) | **GET** /api/v1/datasets | DatasetController@index|
|[**fetchAllDatasetsV2**](#fetchalldatasetsv2) | **GET** /api/v2/datasets | DatasetController@index|
|[**fetchDatasets**](#fetchdatasets) | **GET** /api/v1/datasets/{id} | DatasetController@show|
|[**fetchDatasetsV2**](#fetchdatasetsv2) | **GET** /api/v2/datasets/{id} | DatasetController@showActive|
|[**patchDatasets**](#patchdatasets) | **PATCH** /api/v1/datasets/{id} | DatasetController@edit|
|[**patchDatasetsV2**](#patchdatasetsv2) | **PATCH** /api/v2/datasets/{id} | DatasetController@edit|
|[**patchTeamDatasetsV2**](#patchteamdatasetsv2) | **PATCH** /api/v2/teams/{teamId}/datasets/{id} | TeamDatasetController@edit|
|[**updateDatasets**](#updatedatasets) | **PUT** /api/v1/datasets/{id} | DatasetController@update|
|[**updateDatasetsV2**](#updatedatasetsv2) | **PUT** /api/v2/datasets/{id} | DatasetController@update|
|[**updateTeamDatasetsV2**](#updateteamdatasetsv2) | **PUT** /api/v2/teams/{teamId}/datasets/{id} | TeamDatasetController@update|

# **countUniqueFields**
> CountUniqueFieldsCollections200Response countUniqueFields()

Get Counts for distinct entries of a field in the model

### Example

```typescript
import {
    DatasetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let field: string; //name of the field to perform a count on (default to undefined)
let teamId: number; //team id (default to undefined)

const { status, data } = await apiInstance.countUniqueFields(
    field,
    teamId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **field** | [**string**] | name of the field to perform a count on | defaults to undefined|
| **teamId** | [**number**] | team id | defaults to undefined|


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

# **createDatasets**
> CreateDarIntegration201Response createDatasets(createDatasetsRequest)

Create a new dataset

### Example

```typescript
import {
    DatasetsApi,
    Configuration,
    CreateDatasetsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let createDatasetsRequest: CreateDatasetsRequest; //Pass user credentials

const { status, data } = await apiInstance.createDatasets(
    createDatasetsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createDatasetsRequest** | **CreateDatasetsRequest**| Pass user credentials | |


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

# **createDatasetsV2**
> CreateDarIntegration201Response createDatasetsV2(updateDatasetsRequest)

Create a new dataset

### Example

```typescript
import {
    DatasetsApi,
    Configuration,
    UpdateDatasetsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let updateDatasetsRequest: UpdateDatasetsRequest; //Pass user credentials

const { status, data } = await apiInstance.createDatasetsV2(
    updateDatasetsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateDatasetsRequest** | **UpdateDatasetsRequest**| Pass user credentials | |


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

# **createTeamDatasetsV2**
> CreateDarIntegration201Response createTeamDatasetsV2(patchDatasetsV2Request)

Create a new dataset for a team

### Example

```typescript
import {
    DatasetsApi,
    Configuration,
    PatchDatasetsV2Request
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let teamId: number; //team id (default to undefined)
let patchDatasetsV2Request: PatchDatasetsV2Request; //Pass user credentials

const { status, data } = await apiInstance.createTeamDatasetsV2(
    teamId,
    patchDatasetsV2Request
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **patchDatasetsV2Request** | **PatchDatasetsV2Request**| Pass user credentials | |
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

# **deleteDatasets**
> DeleteApplications200Response deleteDatasets()

Delete a dataset

### Example

```typescript
import {
    DatasetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let id: number; //dataset id (default to undefined)

const { status, data } = await apiInstance.deleteDatasets(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | dataset id | defaults to undefined|


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

# **deleteDatasetsV2**
> DeleteApplications200Response deleteDatasetsV2()

Delete a dataset

### Example

```typescript
import {
    DatasetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let id: number; //dataset id (default to undefined)

const { status, data } = await apiInstance.deleteDatasetsV2(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | dataset id | defaults to undefined|


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

# **deleteTeamDatasetsV2**
> DeleteApplications200Response deleteTeamDatasetsV2()

Delete a team\'s dataset

### Example

```typescript
import {
    DatasetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //dataset id (default to undefined)

const { status, data } = await apiInstance.deleteTeamDatasetsV2(
    teamId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | dataset id | defaults to undefined|


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

# **exportDatasetMetadata**
> string exportDatasetMetadata()

Export Structural Metadata CSV of a single dataset

### Example

```typescript
import {
    DatasetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let id: number; //dataset id (default to undefined)
let downloadType: string; //download type (default to undefined)

const { status, data } = await apiInstance.exportDatasetMetadata(
    id,
    downloadType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | dataset id | defaults to undefined|
| **downloadType** | [**string**] | download type | defaults to undefined|


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
|**400** | Bad request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **exportDatasets**
> string exportDatasets()

Export CSV Of All Datasets

### Example

```typescript
import {
    DatasetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let teamId: number; //team id (default to undefined)
let datasetId: number; //dataset id (optional) (default to undefined)

const { status, data } = await apiInstance.exportDatasets(
    teamId,
    datasetId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|
| **datasetId** | [**number**] | dataset id | (optional) defaults to undefined|


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

# **exportDur**
> string exportDur()

Export CSV Of All Dur\'s

### Example

```typescript
import {
    DatasetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let teamId: number; //team id (default to undefined)
let durId: number; //dur id (optional) (default to undefined)

const { status, data } = await apiInstance.exportDur(
    teamId,
    durId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|
| **durId** | [**number**] | dur id | (optional) defaults to undefined|


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

# **exportMockDataset**
> string exportMockDataset()

Export Mock

### Example

```typescript
import {
    DatasetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let type: 'template_dataset_structural_metadata' | 'dataset_metadata'; //type export (default to undefined)

const { status, data } = await apiInstance.exportMockDataset(
    type
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **type** | [**&#39;template_dataset_structural_metadata&#39; | &#39;dataset_metadata&#39;**]**Array<&#39;template_dataset_structural_metadata&#39; &#124; &#39;dataset_metadata&#39;>** | type export | defaults to undefined|


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
|**404** | File Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **exportMockDatasetV2**
> string exportMockDatasetV2()

Export Mock

### Example

```typescript
import {
    DatasetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let type: 'template_dataset_structural_metadata' | 'dataset_metadata'; // (default to undefined)

const { status, data } = await apiInstance.exportMockDatasetV2(
    type
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **type** | [**&#39;template_dataset_structural_metadata&#39; | &#39;dataset_metadata&#39;**]**Array<&#39;template_dataset_structural_metadata&#39; &#124; &#39;dataset_metadata&#39;>** |  | defaults to undefined|


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
|**404** | File Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchAllDatasets**
> FetchAllDatasets200Response fetchAllDatasets()

Get All Datasets

### Example

```typescript
import {
    DatasetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let teamId: number; //team id (default to undefined)
let pid: string; //get based on a pid (optional) (default to undefined)
let sort: string; //Field and direction (colon separated) to sort by (default: \'created:desc\') ... <br/> <br/>         - ?sort=\\<field\\>:\\<direction\\> <br/>         - \\<direction\\> can only be \'asc\' or \'desc\'  <br/>         - \\<field\\> can only be a valid field for the dataset table that can be ordered on  <br/>         - \\<field\\> can start with the prefix \'metadata.\' so that nested values within the field \'metadata\'  <br/>             (represented by the GWDM JSON structure) can be used to order on.  <br/>  <br/> (optional) (default to undefined)
let title: string; //Three or more characters to filter dataset titles by (optional) (default to undefined)
let status: string; //Dataset status to filter by (\'ACTIVE\', \'DRAFT\', \'ARCHIVED\') (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllDatasets(
    teamId,
    pid,
    sort,
    title,
    status
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | team id | defaults to undefined|
| **pid** | [**string**] | get based on a pid | (optional) defaults to undefined|
| **sort** | [**string**] | Field and direction (colon separated) to sort by (default: \&#39;created:desc\&#39;) ... &lt;br/&gt; &lt;br/&gt;         - ?sort&#x3D;\\&lt;field\\&gt;:\\&lt;direction\\&gt; &lt;br/&gt;         - \\&lt;direction\\&gt; can only be \&#39;asc\&#39; or \&#39;desc\&#39;  &lt;br/&gt;         - \\&lt;field\\&gt; can only be a valid field for the dataset table that can be ordered on  &lt;br/&gt;         - \\&lt;field\\&gt; can start with the prefix \&#39;metadata.\&#39; so that nested values within the field \&#39;metadata\&#39;  &lt;br/&gt;             (represented by the GWDM JSON structure) can be used to order on.  &lt;br/&gt;  &lt;br/&gt; | (optional) defaults to undefined|
| **title** | [**string**] | Three or more characters to filter dataset titles by | (optional) defaults to undefined|
| **status** | [**string**] | Dataset status to filter by (\&#39;ACTIVE\&#39;, \&#39;DRAFT\&#39;, \&#39;ARCHIVED\&#39;) | (optional) defaults to undefined|


### Return type

**FetchAllDatasets200Response**

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

# **fetchAllDatasetsV2**
> FetchAllDatasets200Response fetchAllDatasetsV2()

Returns a list of all datasets

### Example

```typescript
import {
    DatasetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let sort: string; //Field and direction (colon separated) to sort by (default: \'created:desc\') ... <br/> <br/>         - ?sort=\\<field\\>:\\<direction\\> <br/>         - \\<direction\\> can only be \'asc\' or \'desc\'  <br/>         - \\<field\\> can only be a valid field for the dataset table that can be ordered on  <br/>         - \\<field\\> can start with the prefix \'metadata.\' so that nested values within the field \'metadata\'  <br/>             (represented by the GWDM JSON structure) can be used to order on.  <br/>  <br/> (optional) (default to undefined)
let title: string; //Three or more characters to filter dataset titles by (optional) (default to undefined)
let status: string; //Dataset status to filter by (\'ACTIVE\', \'DRAFT\', \'ARCHIVED\') (optional) (default to undefined)
let withMetadata: string; //Boolean whether to return dataset metadata (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllDatasetsV2(
    sort,
    title,
    status,
    withMetadata
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sort** | [**string**] | Field and direction (colon separated) to sort by (default: \&#39;created:desc\&#39;) ... &lt;br/&gt; &lt;br/&gt;         - ?sort&#x3D;\\&lt;field\\&gt;:\\&lt;direction\\&gt; &lt;br/&gt;         - \\&lt;direction\\&gt; can only be \&#39;asc\&#39; or \&#39;desc\&#39;  &lt;br/&gt;         - \\&lt;field\\&gt; can only be a valid field for the dataset table that can be ordered on  &lt;br/&gt;         - \\&lt;field\\&gt; can start with the prefix \&#39;metadata.\&#39; so that nested values within the field \&#39;metadata\&#39;  &lt;br/&gt;             (represented by the GWDM JSON structure) can be used to order on.  &lt;br/&gt;  &lt;br/&gt; | (optional) defaults to undefined|
| **title** | [**string**] | Three or more characters to filter dataset titles by | (optional) defaults to undefined|
| **status** | [**string**] | Dataset status to filter by (\&#39;ACTIVE\&#39;, \&#39;DRAFT\&#39;, \&#39;ARCHIVED\&#39;) | (optional) defaults to undefined|
| **withMetadata** | [**string**] | Boolean whether to return dataset metadata | (optional) defaults to undefined|


### Return type

**FetchAllDatasets200Response**

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

# **fetchDatasets**
> FetchDatasets200Response fetchDatasets()

Get dataset by id

### Example

```typescript
import {
    DatasetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let id: number; //dataset id (default to undefined)
let _export: string; //Alternative output schema model. (optional) (default to undefined)
let schemaModel: string; //Alternative output schema model. (optional) (default to undefined)
let schemaVersion: string; //Alternative output schema version. (optional) (default to undefined)

const { status, data } = await apiInstance.fetchDatasets(
    id,
    _export,
    schemaModel,
    schemaVersion
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | dataset id | defaults to undefined|
| **_export** | [**string**] | Alternative output schema model. | (optional) defaults to undefined|
| **schemaModel** | [**string**] | Alternative output schema model. | (optional) defaults to undefined|
| **schemaVersion** | [**string**] | Alternative output schema version. | (optional) defaults to undefined|


### Return type

**FetchDatasets200Response**

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

# **fetchDatasetsV2**
> FetchDatasets200Response fetchDatasetsV2()

Get publicly visible dataset by id

### Example

```typescript
import {
    DatasetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let id: number; //dataset id (default to undefined)
let _export: string; //Set to \'structuralMetadata\' to download as CSV. (optional) (default to undefined)
let schemaModel: string; //Alternative output schema model. (optional) (default to undefined)
let schemaVersion: string; //Alternative output schema version. (optional) (default to undefined)

const { status, data } = await apiInstance.fetchDatasetsV2(
    id,
    _export,
    schemaModel,
    schemaVersion
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | dataset id | defaults to undefined|
| **_export** | [**string**] | Set to \&#39;structuralMetadata\&#39; to download as CSV. | (optional) defaults to undefined|
| **schemaModel** | [**string**] | Alternative output schema model. | (optional) defaults to undefined|
| **schemaVersion** | [**string**] | Alternative output schema version. | (optional) defaults to undefined|


### Return type

**FetchDatasets200Response**

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

# **patchDatasets**
> DeleteApplications200Response patchDatasets()

Patch dataset by id

### Example

```typescript
import {
    DatasetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let id: number; //dataset id (default to undefined)
let unarchive: string; //Unarchive a dataset (optional) (default to undefined)

const { status, data } = await apiInstance.patchDatasets(
    id,
    unarchive
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | dataset id | defaults to undefined|
| **unarchive** | [**string**] | Unarchive a dataset | (optional) defaults to undefined|


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
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patchDatasetsV2**
> DeleteApplications200Response patchDatasetsV2(patchDatasetsV2Request)

Patch dataset by id

### Example

```typescript
import {
    DatasetsApi,
    Configuration,
    PatchDatasetsV2Request
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let id: number; //dataset id (default to undefined)
let patchDatasetsV2Request: PatchDatasetsV2Request; //

const { status, data } = await apiInstance.patchDatasetsV2(
    id,
    patchDatasetsV2Request
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **patchDatasetsV2Request** | **PatchDatasetsV2Request**|  | |
| **id** | [**number**] | dataset id | defaults to undefined|


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
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patchTeamDatasetsV2**
> DeleteApplications200Response patchTeamDatasetsV2(patchDatasetsV2Request)

Edit a dataset owned by a team

### Example

```typescript
import {
    DatasetsApi,
    Configuration,
    PatchDatasetsV2Request
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //dataset id (default to undefined)
let patchDatasetsV2Request: PatchDatasetsV2Request; //Pass user credentials

const { status, data } = await apiInstance.patchTeamDatasetsV2(
    teamId,
    id,
    patchDatasetsV2Request
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **patchDatasetsV2Request** | **PatchDatasetsV2Request**| Pass user credentials | |
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | dataset id | defaults to undefined|


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
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateDatasets**
> CreateDarIntegration201Response updateDatasets(updateDatasetsRequest)

Update a dataset with a new dataset version

### Example

```typescript
import {
    DatasetsApi,
    Configuration,
    UpdateDatasetsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let id: number; //dataset id (default to undefined)
let updateDatasetsRequest: UpdateDatasetsRequest; //Pass user credentials

const { status, data } = await apiInstance.updateDatasets(
    id,
    updateDatasetsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateDatasetsRequest** | **UpdateDatasetsRequest**| Pass user credentials | |
| **id** | [**number**] | dataset id | defaults to undefined|


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

# **updateDatasetsV2**
> CreateDarIntegration201Response updateDatasetsV2(updateDatasetsRequest)

Update a dataset with a new dataset version

### Example

```typescript
import {
    DatasetsApi,
    Configuration,
    UpdateDatasetsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let id: number; //dataset id (default to undefined)
let updateDatasetsRequest: UpdateDatasetsRequest; //

const { status, data } = await apiInstance.updateDatasetsV2(
    id,
    updateDatasetsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateDatasetsRequest** | **UpdateDatasetsRequest**|  | |
| **id** | [**number**] | dataset id | defaults to undefined|


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

# **updateTeamDatasetsV2**
> CreateDarIntegration201Response updateTeamDatasetsV2(patchDatasetsV2Request)

Update a team dataset with a new dataset version

### Example

```typescript
import {
    DatasetsApi,
    Configuration,
    PatchDatasetsV2Request
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DatasetsApi(configuration);

let teamId: number; //team id (default to undefined)
let id: number; //dataset id (default to undefined)
let patchDatasetsV2Request: PatchDatasetsV2Request; //Pass user credentials

const { status, data } = await apiInstance.updateTeamDatasetsV2(
    teamId,
    id,
    patchDatasetsV2Request
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **patchDatasetsV2Request** | **PatchDatasetsV2Request**| Pass user credentials | |
| **teamId** | [**number**] | team id | defaults to undefined|
| **id** | [**number**] | dataset id | defaults to undefined|


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

