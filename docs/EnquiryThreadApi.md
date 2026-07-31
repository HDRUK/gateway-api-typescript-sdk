# EnquiryThreadApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createEnquiryThreads**](#createenquirythreads) | **POST** /api/v1/enquiry_threads | EnquiryThread@store|
|[**fetchAllEnquiryThreads**](#fetchallenquirythreads) | **GET** /api/v1/enquiry_threads | EnquiryThread@index|
|[**fetchEnquiryThreads**](#fetchenquirythreads) | **GET** /api/v1/enquiry_threads/{id} | EnquiryThread@show|

# **createEnquiryThreads**
> CreateCategories200Response createEnquiryThreads(createEnquiryThreadsRequest)

Creates one or more new EnquiryThreads

### Example

```typescript
import {
    EnquiryThreadApi,
    Configuration,
    CreateEnquiryThreadsRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new EnquiryThreadApi(configuration);

let createEnquiryThreadsRequest: CreateEnquiryThreadsRequest; //EnquiryThread definition

const { status, data } = await apiInstance.createEnquiryThreads(
    createEnquiryThreadsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createEnquiryThreadsRequest** | **CreateEnquiryThreadsRequest**| EnquiryThread definition | |


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

# **fetchAllEnquiryThreads**
> FetchAllEnquiryThreads200Response fetchAllEnquiryThreads()

Returns a list of EnquiryThreads from the system

### Example

```typescript
import {
    EnquiryThreadApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new EnquiryThreadApi(configuration);

let perPage: number; //per page (optional) (default to undefined)

const { status, data } = await apiInstance.fetchAllEnquiryThreads(
    perPage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **perPage** | [**number**] | per page | (optional) defaults to undefined|


### Return type

**FetchAllEnquiryThreads200Response**

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

# **fetchEnquiryThreads**
> FetchAllEnquiryThreads200Response fetchEnquiryThreads()

Return a single EnquiryThread

### Example

```typescript
import {
    EnquiryThreadApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new EnquiryThreadApi(configuration);

let id: number; //EnquiryThread id (default to undefined)

const { status, data } = await apiInstance.fetchEnquiryThreads(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | EnquiryThread id | defaults to undefined|


### Return type

**FetchAllEnquiryThreads200Response**

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

