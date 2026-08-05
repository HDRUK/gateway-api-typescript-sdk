# ReviewsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**deleteReviews**](#deletereviews) | **DELETE** /api/v1/reviews/{id} | Delete a review|
|[**editReviews**](#editreviews) | **PATCH** /api/v1/reviews/{id} | Edit a review|
|[**updateReviews**](#updatereviews) | **PUT** /api/v1/reviews/{id} | Update a review|

# **deleteReviews**
> DeleteApplications200Response deleteReviews()

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

# **editReviews**
> UpdateReviews200Response editReviews(updateReviewsRequest)

Edit a review

### Example

```typescript
import {
    ReviewsApi,
    Configuration,
    UpdateReviewsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ReviewsApi(configuration);

let id: number; //review id (default to undefined)
let updateReviewsRequest: UpdateReviewsRequest; //Pass user credentials

const { status, data } = await apiInstance.editReviews(
    id,
    updateReviewsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateReviewsRequest** | **UpdateReviewsRequest**| Pass user credentials | |
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

# **updateReviews**
> UpdateReviews200Response updateReviews(updateReviewsRequest)

Update a review

### Example

```typescript
import {
    ReviewsApi,
    Configuration,
    UpdateReviewsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new ReviewsApi(configuration);

let id: number; //review id (default to undefined)
let updateReviewsRequest: UpdateReviewsRequest; //Pass user credentials

const { status, data } = await apiInstance.updateReviews(
    id,
    updateReviewsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateReviewsRequest** | **UpdateReviewsRequest**| Pass user credentials | |
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

