# DataAccessTemplatesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**darTemplateCountUniqueFields**](#dartemplatecountuniquefields) | **GET** /api/v1/dar/templates/count/{field} | DataAccessTemplateController@count|

# **darTemplateCountUniqueFields**
> CountUniqueFieldsCollections200Response darTemplateCountUniqueFields()

Get Counts for distinct entries of a field in the model

### Example

```typescript
import {
    DataAccessTemplatesApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new DataAccessTemplatesApi(configuration);

let field: string; //name of the field to perform a count on (default to undefined)

const { status, data } = await apiInstance.darTemplateCountUniqueFields(
    field
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **field** | [**string**] | name of the field to perform a count on | defaults to undefined|


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

