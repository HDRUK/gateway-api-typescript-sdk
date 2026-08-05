# WidgetsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createWidget**](#createwidget) | **POST** /api/v1/teams/{teamId}/widgets | Create a new widget|
|[**deleteWidget**](#deletewidget) | **DELETE** /api/v1/teams/{teamId}/widgets/{id} | Delete a widget|
|[**fetchAllWidgets**](#fetchallwidgets) | **GET** /api/v1/teams/{teamId}/widgets | WidgetController@index|
|[**fetchWidget**](#fetchwidget) | **GET** /api/v1/teams/{teamId}/widgets/{id} | WidgetController@retrieve|
|[**fetchWidgetDataSources**](#fetchwidgetdatasources) | **GET** /api/v1/teams/{teamId}/widgets/data | WidgetController@getWidgetData|
|[**retrieveWidgetData**](#retrievewidgetdata) | **GET** /api/v1/teams/{teamId}/widgets/{id}/data | Retrieve data related to a widget|
|[**trackWidgetEvent**](#trackwidgetevent) | **POST** /api/v1/teams/{teamId}/widgets/{id}/track | Record a widget analytics event|
|[**updateWidget**](#updatewidget) | **PATCH** /api/v1/teams/{teamId}/widgets/{id} | Update an existing widget|
|[**widgetAnalytics**](#widgetanalytics) | **GET** /api/v1/teams/{teamId}/widgets/analytics | Get widget analytics for a team|

# **createWidget**
> CreateWidget201Response createWidget(createWidgetRequest)

Creates a new widget for a given team

### Example

```typescript
import {
    WidgetsApi,
    Configuration,
    CreateWidgetRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new WidgetsApi(configuration);

let teamId: number; //Team ID the widget belongs to (default to undefined)
let createWidgetRequest: CreateWidgetRequest; //

const { status, data } = await apiInstance.createWidget(
    teamId,
    createWidgetRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createWidgetRequest** | **CreateWidgetRequest**|  | |
| **teamId** | [**number**] | Team ID the widget belongs to | defaults to undefined|


### Return type

**CreateWidget201Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Widget created successfully |  -  |
|**400** | Validation failed |  -  |
|**500** | Server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteWidget**
> DeleteApplications200Response deleteWidget()

Soft delete a widget belonging to a specific team

### Example

```typescript
import {
    WidgetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new WidgetsApi(configuration);

let teamId: number; //Team ID (default to undefined)
let id: number; //Widget ID (default to undefined)

const { status, data } = await apiInstance.deleteWidget(
    teamId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team ID | defaults to undefined|
| **id** | [**number**] | Widget ID | defaults to undefined|


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
|**404** | Widget not found |  -  |
|**200** | Widget deleted successfully |  -  |
|**500** | Server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchAllWidgets**
> FetchAllWidgets200Response fetchAllWidgets()

Get All Widgets

### Example

```typescript
import {
    WidgetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new WidgetsApi(configuration);

let teamId: number; //Team ID (default to undefined)

const { status, data } = await apiInstance.fetchAllWidgets(
    teamId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team ID | defaults to undefined|


### Return type

**FetchAllWidgets200Response**

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

# **fetchWidget**
> FetchWidget200Response fetchWidget()

Get a single Widget

### Example

```typescript
import {
    WidgetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new WidgetsApi(configuration);

let teamId: number; //Team ID (default to undefined)
let id: number; //Widget ID (default to undefined)

const { status, data } = await apiInstance.fetchWidget(
    teamId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team ID | defaults to undefined|
| **id** | [**number**] | Widget ID | defaults to undefined|


### Return type

**FetchWidget200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**404** | Widget not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchWidgetDataSources**
> FetchWidgetDataSources200Response fetchWidgetDataSources()

Fetch lightweight data (id, name, etc.) for multiple teams across datasets, tools, collections, and DURS

### Example

```typescript
import {
    WidgetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new WidgetsApi(configuration);

let teamId: number; //Team ID (default to undefined)
let teamIds: string; //Comma-separated list of team IDs to filter data (default to undefined)

const { status, data } = await apiInstance.fetchWidgetDataSources(
    teamId,
    teamIds
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team ID | defaults to undefined|
| **teamIds** | [**string**] | Comma-separated list of team IDs to filter data | defaults to undefined|


### Return type

**FetchWidgetDataSources200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Aggregated data retrieved successfully |  -  |
|**400** | Invalid or missing teamIds parameter |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **retrieveWidgetData**
> RetrieveWidgetData200Response retrieveWidgetData()

Fetches datasets, data uses, scripts, and collections linked to a widget

### Example

```typescript
import {
    WidgetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new WidgetsApi(configuration);

let teamId: number; //Team ID (default to undefined)
let id: number; //Widget ID (default to undefined)
let domainOrigin: string; //Optional domain URL to check against the widget\'s permitted_domains list (default to undefined)

const { status, data } = await apiInstance.retrieveWidgetData(
    teamId,
    id,
    domainOrigin
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team ID | defaults to undefined|
| **id** | [**number**] | Widget ID | defaults to undefined|
| **domainOrigin** | [**string**] | Optional domain URL to check against the widget\&#39;s permitted_domains list | defaults to undefined|


### Return type

**RetrieveWidgetData200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**403** | Forbidden — domain not permitted for this widget |  -  |
|**200** | Widget data retrieved successfully |  -  |
|**404** | Widget not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **trackWidgetEvent**
> trackWidgetEvent(trackWidgetEventRequest)

Public endpoint for frontend clients to record user interactions with a widget (page views, code copies, gateway clicks, searches). No authentication required.

### Example

```typescript
import {
    WidgetsApi,
    Configuration,
    TrackWidgetEventRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new WidgetsApi(configuration);

let teamId: number; // (default to undefined)
let id: number; // (default to undefined)
let trackWidgetEventRequest: TrackWidgetEventRequest; //

const { status, data } = await apiInstance.trackWidgetEvent(
    teamId,
    id,
    trackWidgetEventRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **trackWidgetEventRequest** | **TrackWidgetEventRequest**|  | |
| **teamId** | [**number**] |  | defaults to undefined|
| **id** | [**number**] |  | defaults to undefined|


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | Event recorded |  -  |
|**404** | Widget not found |  -  |
|**422** | Validation error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateWidget**
> UpdateWidget200Response updateWidget()

Updates an existing widget for a given team ID

### Example

```typescript
import {
    WidgetsApi,
    Configuration,
    UpdateWidgetRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new WidgetsApi(configuration);

let teamId: number; //Team ID (default to undefined)
let id: number; //Widget ID (default to undefined)
let updateWidgetRequest: UpdateWidgetRequest; // (optional)

const { status, data } = await apiInstance.updateWidget(
    teamId,
    id,
    updateWidgetRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateWidgetRequest** | **UpdateWidgetRequest**|  | |
| **teamId** | [**number**] | Team ID | defaults to undefined|
| **id** | [**number**] | Widget ID | defaults to undefined|


### Return type

**UpdateWidget200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Widget successfully updated |  -  |
|**404** | Widget not found |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **widgetAnalytics**
> WidgetAnalytics200Response widgetAnalytics()

Returns aggregated event counts per widget, per event type, and over time. Supports date range filtering and time-based grouping.

### Example

```typescript
import {
    WidgetsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new WidgetsApi(configuration);

let teamId: number; // (default to undefined)
let from: string; //Start date (Y-m-d) (optional) (default to undefined)
let to: string; //End date (Y-m-d) (optional) (default to undefined)
let groupBy: 'day' | 'week' | 'month'; //Time granularity (optional) (default to 'day')

const { status, data } = await apiInstance.widgetAnalytics(
    teamId,
    from,
    to,
    groupBy
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] |  | defaults to undefined|
| **from** | [**string**] | Start date (Y-m-d) | (optional) defaults to undefined|
| **to** | [**string**] | End date (Y-m-d) | (optional) defaults to undefined|
| **groupBy** | [**&#39;day&#39; | &#39;week&#39; | &#39;month&#39;**]**Array<&#39;day&#39; &#124; &#39;week&#39; &#124; &#39;month&#39;>** | Time granularity | (optional) defaults to 'day'|


### Return type

**WidgetAnalytics200Response**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Analytics data |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

