# ReviewsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createReviews**](#createreviews) | **POST** /api/v1/reviews | ReviewController@store|
|[**deleteReviews**](#deletereviews) | **DELETE** /api/v1/reviews/{id} | Delete a review|
|[**editReviews**](#editreviews) | **PATCH** /api/v1/reviews/{id} | Edit a review|
|[**fetchAllReviews**](#fetchallreviews) | **GET** /api/v1/reviews | ReviewController@index|
|[**fetchReviews**](#fetchreviews) | **GET** /api/v1/reviews/{id} | ReviewController@show|
|[**updateReviews**](#updatereviews) | **PUT** /api/v1/reviews/{id} | Update a review|

# **createReviews**
> CreateCategories200Response createReviews(createReviewsRequest)

Create a new review

### Example

```typescript
import {
    ReviewsApi,
    Configuration,
    CreateReviewsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ReviewsApi(configuration);

let createReviewsRequest: CreateReviewsRequest; //Pass user credentials

const { status, data } = await apiInstance.createReviews(
    createReviewsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createReviewsRequest** | **CreateReviewsRequest**| Pass user credentials | |


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
|**201** | Created |  -  |
|**401** | Unauthorized |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteReviews**
> DeleteAliases200Response deleteReviews()

Delete a review

### Example

```typescript
import {
    ReviewsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ReviewsApi(configuration);

let id: number; //review id (default to undefined)

const { status, data } = await apiInstance.deleteReviews(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | review id | defaults to undefined|


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

# **editReviews**
> UpdateReviews200Response editReviews(createReviewsRequest)

Edit a review

### Example

```typescript
import {
    ReviewsApi,
    Configuration,
    CreateReviewsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ReviewsApi(configuration);

let id: number; //review id (default to undefined)
let createReviewsRequest: CreateReviewsRequest; //Pass user credentials

const { status, data } = await apiInstance.editReviews(
    id,
    createReviewsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createReviewsRequest** | **CreateReviewsRequest**| Pass user credentials | |
| **id** | [**number**] | review id | defaults to undefined|


### Return type

**UpdateReviews200Response**

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

# **fetchAllReviews**
> FetchAllReviews200Response fetchAllReviews()

Get All Reviews

### Example

```typescript
import {
    ReviewsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ReviewsApi(configuration);

const { status, data } = await apiInstance.fetchAllReviews();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**FetchAllReviews200Response**

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

# **fetchReviews**
> FetchAllReviews200Response fetchReviews()

Get review by id

### Example

```typescript
import {
    ReviewsApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ReviewsApi(configuration);

let id: number; //review id (default to undefined)

const { status, data } = await apiInstance.fetchReviews(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | review id | defaults to undefined|


### Return type

**FetchAllReviews200Response**

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

# **updateReviews**
> UpdateReviews200Response updateReviews(createReviewsRequest)

Update a review

### Example

```typescript
import {
    ReviewsApi,
    Configuration,
    CreateReviewsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ReviewsApi(configuration);

let id: number; //review id (default to undefined)
let createReviewsRequest: CreateReviewsRequest; //Pass user credentials

const { status, data } = await apiInstance.updateReviews(
    id,
    createReviewsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createReviewsRequest** | **CreateReviewsRequest**| Pass user credentials | |
| **id** | [**number**] | review id | defaults to undefined|


### Return type

**UpdateReviews200Response**

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

