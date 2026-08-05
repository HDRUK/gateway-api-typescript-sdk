# DataAccessApplicationReviewApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createTeamDarApplicationQuestionReview**](#createteamdarapplicationquestionreview) | **POST** /api/v1/teams/{team_id}/dar/applications/{id}/questions/{questionId}/reviews | DataAccessApplicationReview@store|
|[**createTeamDarApplicationReview**](#createteamdarapplicationreview) | **POST** /api/v1/teams/{team_id}/dar/applications/{id}/reviews | DataAccessApplicationReview@storeGlobal|
|[**deleteTeamDarApplicationReviewFile**](#deleteteamdarapplicationreviewfile) | **DELETE** /api/v1/teams/{teamId}/dar/applications/{id}/reviews/{reviewId}/files/{fileId} | DataAccessApplicationReview@destroyFile|
|[**fetchTeamDarApplicationReviewFile**](#fetchteamdarapplicationreviewfile) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/reviews/{reviewId}/download/{fileId} | DataAccessApplicationReview@downloadFile|
|[**fetchTeamDarApplicationReviews**](#fetchteamdarapplicationreviews) | **GET** /api/v1/teams/{team_id}/dar/applications/{id}/reviews | DataAccessApplicationReview@index|
|[**updateTeamDarApplicationQuestionReview**](#updateteamdarapplicationquestionreview) | **PUT** /api/v1/teams/{team_id}/dar/applications/{id}/questions/{questionId}/reviews/{reviewId} | DataAccessApplicationReview@update|
|[**updateTeamDarApplicationReview**](#updateteamdarapplicationreview) | **PUT** /api/v1/teams/{team_id}/dar/applications/{id}/reviews/{reviewId} | DataAccessApplicationReview@updateGlobal|

# **createTeamDarApplicationQuestionReview**
> CreateDarIntegration201Response createTeamDarApplicationQuestionReview(createTeamDarApplicationReviewRequest)

Create a new review comment on a question in a DAR application

### Example

```typescript
import {
    DataAccessApplicationReviewApi,
    Configuration,
    CreateTeamDarApplicationReviewRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationReviewApi(configuration);

let teamId: number; //Team id (default to undefined)
let id: number; //DAR application id (default to undefined)
let questionId: number; //DAR application question id (default to undefined)
let createTeamDarApplicationReviewRequest: CreateTeamDarApplicationReviewRequest; //DataAccessApplicationReview definition

const { status, data } = await apiInstance.createTeamDarApplicationQuestionReview(
    teamId,
    id,
    questionId,
    createTeamDarApplicationReviewRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createTeamDarApplicationReviewRequest** | **CreateTeamDarApplicationReviewRequest**| DataAccessApplicationReview definition | |
| **teamId** | [**number**] | Team id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|
| **questionId** | [**number**] | DAR application question id | defaults to undefined|


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
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createTeamDarApplicationReview**
> CreateDarIntegration201Response createTeamDarApplicationReview(createTeamDarApplicationReviewRequest)

Create a new review comment on a DAR application

### Example

```typescript
import {
    DataAccessApplicationReviewApi,
    Configuration,
    CreateTeamDarApplicationReviewRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationReviewApi(configuration);

let teamId: number; //Team id (default to undefined)
let id: number; //DAR application id (default to undefined)
let createTeamDarApplicationReviewRequest: CreateTeamDarApplicationReviewRequest; //DataAccessApplicationReview definition

const { status, data } = await apiInstance.createTeamDarApplicationReview(
    teamId,
    id,
    createTeamDarApplicationReviewRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createTeamDarApplicationReviewRequest** | **CreateTeamDarApplicationReviewRequest**| DataAccessApplicationReview definition | |
| **teamId** | [**number**] | Team id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|


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
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteTeamDarApplicationReviewFile**
> DeleteApplications200Response deleteTeamDarApplicationReviewFile()

Delete a file associated with a DAR review

### Example

```typescript
import {
    DataAccessApplicationReviewApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationReviewApi(configuration);

let teamId: number; //Team id (default to undefined)
let id: number; //Dar application id (default to undefined)
let reviewId: number; //Review id (default to undefined)
let fileId: string; //File uuid (default to undefined)

const { status, data } = await apiInstance.deleteTeamDarApplicationReviewFile(
    teamId,
    id,
    reviewId,
    fileId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team id | defaults to undefined|
| **id** | [**number**] | Dar application id | defaults to undefined|
| **reviewId** | [**number**] | Review id | defaults to undefined|
| **fileId** | [**string**] | File uuid | defaults to undefined|


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

# **fetchTeamDarApplicationReviewFile**
> fetchTeamDarApplicationReviewFile()

Download a file associated with a DAR application review

### Example

```typescript
import {
    DataAccessApplicationReviewApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationReviewApi(configuration);

let teamId: number; //Team id (default to undefined)
let id: number; //DAR application id (default to undefined)
let reviewId: number; //DAR application review id (default to undefined)
let fileId: string; //File uuid (default to undefined)

const { status, data } = await apiInstance.fetchTeamDarApplicationReviewFile(
    teamId,
    id,
    reviewId,
    fileId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|
| **reviewId** | [**number**] | DAR application review id | defaults to undefined|
| **fileId** | [**string**] | File uuid | defaults to undefined|


### Return type

void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: file, application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetchTeamDarApplicationReviews**
> FetchTeamDarApplicationReviews200Response fetchTeamDarApplicationReviews()

Return all reviews on a DAR application

### Example

```typescript
import {
    DataAccessApplicationReviewApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationReviewApi(configuration);

let teamId: number; //Team id (default to undefined)
let id: number; //DAR application id (default to undefined)

const { status, data } = await apiInstance.fetchTeamDarApplicationReviews(
    teamId,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|


### Return type

**FetchTeamDarApplicationReviews200Response**

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

# **updateTeamDarApplicationQuestionReview**
> UpdateTeamDarApplicationQuestionReview200Response updateTeamDarApplicationQuestionReview(createTeamDarApplicationReviewRequest)

Update a review comment on a question in a DAR application

### Example

```typescript
import {
    DataAccessApplicationReviewApi,
    Configuration,
    CreateTeamDarApplicationReviewRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationReviewApi(configuration);

let teamId: number; //Team id (default to undefined)
let id: number; //DAR application id (default to undefined)
let questionId: number; //DAR application question id (default to undefined)
let reviewId: number; //DAR application review id (default to undefined)
let createTeamDarApplicationReviewRequest: CreateTeamDarApplicationReviewRequest; //DataAccessApplicationReview definition

const { status, data } = await apiInstance.updateTeamDarApplicationQuestionReview(
    teamId,
    id,
    questionId,
    reviewId,
    createTeamDarApplicationReviewRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createTeamDarApplicationReviewRequest** | **CreateTeamDarApplicationReviewRequest**| DataAccessApplicationReview definition | |
| **teamId** | [**number**] | Team id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|
| **questionId** | [**number**] | DAR application question id | defaults to undefined|
| **reviewId** | [**number**] | DAR application review id | defaults to undefined|


### Return type

**UpdateTeamDarApplicationQuestionReview200Response**

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

# **updateTeamDarApplicationReview**
> UpdateTeamDarApplicationQuestionReview200Response updateTeamDarApplicationReview(createTeamDarApplicationReviewRequest)

Update a review comment on a DAR application

### Example

```typescript
import {
    DataAccessApplicationReviewApi,
    Configuration,
    CreateTeamDarApplicationReviewRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessApplicationReviewApi(configuration);

let teamId: number; //Team id (default to undefined)
let id: number; //DAR application id (default to undefined)
let reviewId: number; //DAR application review id (default to undefined)
let createTeamDarApplicationReviewRequest: CreateTeamDarApplicationReviewRequest; //DataAccessApplicationReview definition

const { status, data } = await apiInstance.updateTeamDarApplicationReview(
    teamId,
    id,
    reviewId,
    createTeamDarApplicationReviewRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createTeamDarApplicationReviewRequest** | **CreateTeamDarApplicationReviewRequest**| DataAccessApplicationReview definition | |
| **teamId** | [**number**] | Team id | defaults to undefined|
| **id** | [**number**] | DAR application id | defaults to undefined|
| **reviewId** | [**number**] | DAR application review id | defaults to undefined|


### Return type

**UpdateTeamDarApplicationQuestionReview200Response**

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

