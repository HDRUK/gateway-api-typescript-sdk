# TeamDashboardApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**fetchCollectionsViewsV3**](#fetchcollectionsviewsv3) | **GET** /api/v3/teams/{id}/dashboard/collections/views | TeamDashboardController@collectionViews|
|[**fetchDarApplicationsApplicationTimelineV3**](#fetchdarapplicationsapplicationtimelinev3) | **GET** /api/v3/teams/{id}/dar/dashboard/timeline | DataAccessDashboardController@getApplicationTimeline|
|[**fetchDarApplicationsAverageTimeToApprovalV3**](#fetchdarapplicationsaveragetimetoapprovalv3) | **GET** /api/v3/teams/{id}/dar/dashboard/average-time | DataAccessDashboardController@getAverageTimeToApproval|
|[**fetchDarApplicationsCurrentStatusV3**](#fetchdarapplicationscurrentstatusv3) | **GET** /api/v3/teams/{id}/dar/dashboard/status | DataAccessDashboardController@getApplicationStatus|
|[**fetchDarApplicationsDashboardExportCsvV3**](#fetchdarapplicationsdashboardexportcsvv3) | **GET** /api/v3/teams/{id}/dar/dashboard/export/csv | DataAccessDashboardController@exportDashboardCsv|
|[**fetchDarApplicationsDashboardRequiredActionsExportCsvV3**](#fetchdarapplicationsdashboardrequiredactionsexportcsvv3) | **GET** /api/v3/teams/{id}/dar/dashboard/required-actions/export/csv | DataAccessDashboardController@exportRequiredActionsCsv|
|[**fetchDarApplicationsDashboardTimelineExportCsvV3**](#fetchdarapplicationsdashboardtimelineexportcsvv3) | **GET** /api/v3/teams/{id}/dar/dashboard/timeline/export/csv | DataAccessDashboardController@exportDashboardTimelineCsv|
|[**fetchDarApplicationsRequiredActionsV3**](#fetchdarapplicationsrequiredactionsv3) | **GET** /api/v3/teams/{id}/dar/dashboard/required-actions | DataAccessDashboardController@getRequiredActions|
|[**fetchDarMyApplicationsV3**](#fetchdarmyapplicationsv3) | **GET** /api/v3/teams/{id}/dar/dashboard/count | DataAccessDashboardController@getMyApplications|
|[**fetchDashboardDownloadCsvV3**](#fetchdashboarddownloadcsvv3) | **GET** /api/v3/teams/{id}/dashboard/download/csv | TeamDashboardController@downloadCsv|
|[**fetchDataCustodiansViewsV3**](#fetchdatacustodiansviewsv3) | **GET** /api/v3/teams/{id}/dashboard/datacustodians/views | TeamDashboardController@datacustodianViews|
|[**fetchDatasetViews360V3**](#fetchdatasetviews360v3) | **GET** /api/v3/teams/{id}/dashboard/datasets/views/360 | TeamDashboardController@datasetViews360|
|[**fetchDatasetViewsTopV3**](#fetchdatasetviewstopv3) | **GET** /api/v3/teams/{id}/dashboard/datasets/views/top | TeamDashboardController@datasetViewsTop|
|[**fetchEntitiesCountV3**](#fetchentitiescountv3) | **GET** /api/v3/teams/{id}/dashboard/{entity}/count | TeamDashboardController@entityCount|

# **fetchCollectionsViewsV3**
> FetchCollectionsViewsV3200Response fetchCollectionsViewsV3()

Get count of a collection views for a team

### Example

```typescript
import {
    TeamDashboardApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDashboardApi(configuration);

let id: number; //Team ID (default to undefined)
let startDate: string; //Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional) (default to undefined)
let endDate: string; //End date for the reporting interval (Y-m-d). Defaults to today. (optional) (default to undefined)

const { status, data } = await apiInstance.fetchCollectionsViewsV3(
    id,
    startDate,
    endDate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Team ID | defaults to undefined|
| **startDate** | [**string**] | Start date for the reporting interval (Y-m-d). Defaults to one year ago. | (optional) defaults to undefined|
| **endDate** | [**string**] | End date for the reporting interval (Y-m-d). Defaults to today. | (optional) defaults to undefined|


### Return type

**FetchCollectionsViewsV3200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDarApplicationsApplicationTimelineV3**
> CreateWidget201Response fetchDarApplicationsApplicationTimelineV3()

Get Dar applications timeline for a team

### Example

```typescript
import {
    TeamDashboardApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDashboardApi(configuration);

let id: number; //Team ID (default to undefined)
let startDate: string; //Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional) (default to undefined)
let endDate: string; //End date for the reporting interval (Y-m-d). Defaults to today. (optional) (default to undefined)

const { status, data } = await apiInstance.fetchDarApplicationsApplicationTimelineV3(
    id,
    startDate,
    endDate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Team ID | defaults to undefined|
| **startDate** | [**string**] | Start date for the reporting interval (Y-m-d). Defaults to one year ago. | (optional) defaults to undefined|
| **endDate** | [**string**] | End date for the reporting interval (Y-m-d). Defaults to today. | (optional) defaults to undefined|


### Return type

**CreateWidget201Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDarApplicationsAverageTimeToApprovalV3**
> CreateWidget201Response fetchDarApplicationsAverageTimeToApprovalV3()

Get Dar applications average time to approval for a team

### Example

```typescript
import {
    TeamDashboardApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDashboardApi(configuration);

let id: number; //Team ID (default to undefined)
let startDate: string; //Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional) (default to undefined)
let endDate: string; //End date for the reporting interval (Y-m-d). Defaults to today. (optional) (default to undefined)

const { status, data } = await apiInstance.fetchDarApplicationsAverageTimeToApprovalV3(
    id,
    startDate,
    endDate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Team ID | defaults to undefined|
| **startDate** | [**string**] | Start date for the reporting interval (Y-m-d). Defaults to one year ago. | (optional) defaults to undefined|
| **endDate** | [**string**] | End date for the reporting interval (Y-m-d). Defaults to today. | (optional) defaults to undefined|


### Return type

**CreateWidget201Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDarApplicationsCurrentStatusV3**
> CreateWidget201Response fetchDarApplicationsCurrentStatusV3()

Get Dar applications current status for a team

### Example

```typescript
import {
    TeamDashboardApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDashboardApi(configuration);

let id: number; //Team ID (default to undefined)
let startDate: string; //Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional) (default to undefined)
let endDate: string; //End date for the reporting interval (Y-m-d). Defaults to today. (optional) (default to undefined)

const { status, data } = await apiInstance.fetchDarApplicationsCurrentStatusV3(
    id,
    startDate,
    endDate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Team ID | defaults to undefined|
| **startDate** | [**string**] | Start date for the reporting interval (Y-m-d). Defaults to one year ago. | (optional) defaults to undefined|
| **endDate** | [**string**] | End date for the reporting interval (Y-m-d). Defaults to today. | (optional) defaults to undefined|


### Return type

**CreateWidget201Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDarApplicationsDashboardExportCsvV3**
> CreateWidget201Response fetchDarApplicationsDashboardExportCsvV3()

Get Dar applications dashboard export csv for a team

### Example

```typescript
import {
    TeamDashboardApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDashboardApi(configuration);

let id: number; //Team ID (default to undefined)
let startDate: string; //Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional) (default to undefined)
let endDate: string; //End date for the reporting interval (Y-m-d). Defaults to today. (optional) (default to undefined)

const { status, data } = await apiInstance.fetchDarApplicationsDashboardExportCsvV3(
    id,
    startDate,
    endDate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Team ID | defaults to undefined|
| **startDate** | [**string**] | Start date for the reporting interval (Y-m-d). Defaults to one year ago. | (optional) defaults to undefined|
| **endDate** | [**string**] | End date for the reporting interval (Y-m-d). Defaults to today. | (optional) defaults to undefined|


### Return type

**CreateWidget201Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDarApplicationsDashboardRequiredActionsExportCsvV3**
> CreateWidget201Response fetchDarApplicationsDashboardRequiredActionsExportCsvV3()

Get Dar applications dashboard timeline export csv for a team

### Example

```typescript
import {
    TeamDashboardApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDashboardApi(configuration);

let id: number; //Team ID (default to undefined)

const { status, data } = await apiInstance.fetchDarApplicationsDashboardRequiredActionsExportCsvV3(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Team ID | defaults to undefined|


### Return type

**CreateWidget201Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDarApplicationsDashboardTimelineExportCsvV3**
> CreateWidget201Response fetchDarApplicationsDashboardTimelineExportCsvV3()

Get Dar applications dashboard timeline export csv for a team

### Example

```typescript
import {
    TeamDashboardApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDashboardApi(configuration);

let id: number; //Team ID (default to undefined)
let startDate: string; //Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional) (default to undefined)
let endDate: string; //End date for the reporting interval (Y-m-d). Defaults to today. (optional) (default to undefined)

const { status, data } = await apiInstance.fetchDarApplicationsDashboardTimelineExportCsvV3(
    id,
    startDate,
    endDate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Team ID | defaults to undefined|
| **startDate** | [**string**] | Start date for the reporting interval (Y-m-d). Defaults to one year ago. | (optional) defaults to undefined|
| **endDate** | [**string**] | End date for the reporting interval (Y-m-d). Defaults to today. | (optional) defaults to undefined|


### Return type

**CreateWidget201Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDarApplicationsRequiredActionsV3**
> CreateWidget201Response fetchDarApplicationsRequiredActionsV3()

Get Dar applications required actions for a team

### Example

```typescript
import {
    TeamDashboardApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDashboardApi(configuration);

let id: number; //Team ID (default to undefined)
let startDate: string; //Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional) (default to undefined)
let endDate: string; //End date for the reporting interval (Y-m-d). Defaults to today. (optional) (default to undefined)

const { status, data } = await apiInstance.fetchDarApplicationsRequiredActionsV3(
    id,
    startDate,
    endDate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Team ID | defaults to undefined|
| **startDate** | [**string**] | Start date for the reporting interval (Y-m-d). Defaults to one year ago. | (optional) defaults to undefined|
| **endDate** | [**string**] | End date for the reporting interval (Y-m-d). Defaults to today. | (optional) defaults to undefined|


### Return type

**CreateWidget201Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDarMyApplicationsV3**
> CreateWidget201Response fetchDarMyApplicationsV3()

Get Dar applications for a team

### Example

```typescript
import {
    TeamDashboardApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDashboardApi(configuration);

let id: number; //Team ID (default to undefined)
let startDate: string; //Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional) (default to undefined)
let endDate: string; //End date for the reporting interval (Y-m-d). Defaults to today. (optional) (default to undefined)

const { status, data } = await apiInstance.fetchDarMyApplicationsV3(
    id,
    startDate,
    endDate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Team ID | defaults to undefined|
| **startDate** | [**string**] | Start date for the reporting interval (Y-m-d). Defaults to one year ago. | (optional) defaults to undefined|
| **endDate** | [**string**] | End date for the reporting interval (Y-m-d). Defaults to today. | (optional) defaults to undefined|


### Return type

**CreateWidget201Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDashboardDownloadCsvV3**
> File fetchDashboardDownloadCsvV3()

Download dashboard data custodian in csv format

### Example

```typescript
import {
    TeamDashboardApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDashboardApi(configuration);

let id: number; //Team ID (default to undefined)
let startDate: string; //Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional) (default to undefined)
let endDate: string; //End date for the reporting interval (Y-m-d). Defaults to today. (optional) (default to undefined)

const { status, data } = await apiInstance.fetchDashboardDownloadCsvV3(
    id,
    startDate,
    endDate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Team ID | defaults to undefined|
| **startDate** | [**string**] | Start date for the reporting interval (Y-m-d). Defaults to one year ago. | (optional) defaults to undefined|
| **endDate** | [**string**] | End date for the reporting interval (Y-m-d). Defaults to today. | (optional) defaults to undefined|


### Return type

**File**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/csv, application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | CSV file download containing dashboard metrics for the team |  -  |
|**400** | Invalid team ID |  -  |
|**500** | Invalid date interval |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDataCustodiansViewsV3**
> FetchCollectionsViewsV3200Response fetchDataCustodiansViewsV3()

Get count of a data custodian views for a team

### Example

```typescript
import {
    TeamDashboardApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDashboardApi(configuration);

let id: number; //Team ID (default to undefined)
let startDate: string; //Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional) (default to undefined)
let endDate: string; //End date for the reporting interval (Y-m-d). Defaults to today. (optional) (default to undefined)

const { status, data } = await apiInstance.fetchDataCustodiansViewsV3(
    id,
    startDate,
    endDate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Team ID | defaults to undefined|
| **startDate** | [**string**] | Start date for the reporting interval (Y-m-d). Defaults to one year ago. | (optional) defaults to undefined|
| **endDate** | [**string**] | End date for the reporting interval (Y-m-d). Defaults to today. | (optional) defaults to undefined|


### Return type

**FetchCollectionsViewsV3200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDatasetViews360V3**
> FetchDatasetViews360V3200Response fetchDatasetViews360V3()

Get count of a datasets views 360 for a team

### Example

```typescript
import {
    TeamDashboardApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDashboardApi(configuration);

let id: number; //Team ID (default to undefined)
let startDate: string; //Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional) (default to undefined)
let endDate: string; //End date for the reporting interval (Y-m-d). Defaults to today. (optional) (default to undefined)

const { status, data } = await apiInstance.fetchDatasetViews360V3(
    id,
    startDate,
    endDate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Team ID | defaults to undefined|
| **startDate** | [**string**] | Start date for the reporting interval (Y-m-d). Defaults to one year ago. | (optional) defaults to undefined|
| **endDate** | [**string**] | End date for the reporting interval (Y-m-d). Defaults to today. | (optional) defaults to undefined|


### Return type

**FetchDatasetViews360V3200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchDatasetViewsTopV3**
> FetchDatasetViewsTopV3200Response fetchDatasetViewsTopV3()

Get count of a datasets views top for a team

### Example

```typescript
import {
    TeamDashboardApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDashboardApi(configuration);

let id: number; //Team ID (default to undefined)
let startDate: string; //Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional) (default to undefined)
let endDate: string; //End date for the reporting interval (Y-m-d). Defaults to today. (optional) (default to undefined)

const { status, data } = await apiInstance.fetchDatasetViewsTopV3(
    id,
    startDate,
    endDate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Team ID | defaults to undefined|
| **startDate** | [**string**] | Start date for the reporting interval (Y-m-d). Defaults to one year ago. | (optional) defaults to undefined|
| **endDate** | [**string**] | End date for the reporting interval (Y-m-d). Defaults to today. | (optional) defaults to undefined|


### Return type

**FetchDatasetViewsTopV3200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchEntitiesCountV3**
> FetchEntitiesCountV3200Response fetchEntitiesCountV3()

Get count of a specific entity for a team

### Example

```typescript
import {
    TeamDashboardApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new TeamDashboardApi(configuration);

let id: number; //Team ID (default to undefined)
let entity: 'datasets' | 'datauses' | 'tools' | 'collections' | 'general-enquires' | 'fesability-enquires' | 'data-access-requests'; //Entity type to count (default to undefined)
let startDate: string; //Start date for the reporting interval (Y-m-d). Defaults to one year ago. (optional) (default to undefined)
let endDate: string; //End date for the reporting interval (Y-m-d). Defaults to today. (optional) (default to undefined)

const { status, data } = await apiInstance.fetchEntitiesCountV3(
    id,
    entity,
    startDate,
    endDate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Team ID | defaults to undefined|
| **entity** | [**&#39;datasets&#39; | &#39;datauses&#39; | &#39;tools&#39; | &#39;collections&#39; | &#39;general-enquires&#39; | &#39;fesability-enquires&#39; | &#39;data-access-requests&#39;**]**Array<&#39;datasets&#39; &#124; &#39;datauses&#39; &#124; &#39;tools&#39; &#124; &#39;collections&#39; &#124; &#39;general-enquires&#39; &#124; &#39;fesability-enquires&#39; &#124; &#39;data-access-requests&#39;>** | Entity type to count | defaults to undefined|
| **startDate** | [**string**] | Start date for the reporting interval (Y-m-d). Defaults to one year ago. | (optional) defaults to undefined|
| **endDate** | [**string**] | End date for the reporting interval (Y-m-d). Defaults to today. | (optional) defaults to undefined|


### Return type

**FetchEntitiesCountV3200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

