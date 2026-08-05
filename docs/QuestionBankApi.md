# QuestionBankApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createQuestionBankQuestion**](#createquestionbankquestion) | **POST** /api/v1/questions | QuestionBank@store|
|[**deleteQuestionBankQuestion**](#deletequestionbankquestion) | **DELETE** /api/v1/questions/{id} | QuestionBank@destroy|
|[**downloadQuestionBankQuestionFile**](#downloadquestionbankquestionfile) | **GET** /api/v1/questions/{id}/files/{fileId} | QuestionBank@destroyFile|
|[**editQuestionBankQuestion**](#editquestionbankquestion) | **PATCH** /api/v1/questions/{id} | QuestionBank@update|
|[**fetchArchivedQuestionBankQuestions**](#fetcharchivedquestionbankquestions) | **GET** /api/v1/questions/archived | QuestionBank@indexArchived|
|[**fetchCustomQuestionBankQuestions**](#fetchcustomquestionbankquestions) | **GET** /api/v1/questions/custom | QuestionBank@indexCustom|
|[**fetchQuestionBankQuestion**](#fetchquestionbankquestion) | **GET** /api/v1/questions/{id} | QuestionBank@show|
|[**fetchQuestionBankQuestionVersion**](#fetchquestionbankquestionversion) | **GET** /api/v1/questions/version/{id} | QuestionBank@showVersion|
|[**fetchQuestionBankQuestions**](#fetchquestionbankquestions) | **GET** /api/v1/questions | QuestionBank@index|
|[**fetchStandardQuestionBankQuestions**](#fetchstandardquestionbankquestions) | **GET** /api/v1/questions/standard | QuestionBank@indexStandard|
|[**fetchTeamQuestionBankQuestionsBySection**](#fetchteamquestionbankquestionsbysection) | **GET** /api/v1/teams/{teamId}/questions/section/{sectionId} | TeamQuestionBank@indexBySection|
|[**updateQuestionBankQuestion**](#updatequestionbankquestion) | **PUT** /api/v1/questions/{id} | QuestionBank@update|
|[**updateQuestionBankQuestionStatus**](#updatequestionbankquestionstatus) | **PATCH** /api/v1/questions/{id}/{status} | QuestionBank@updateStatus|

# **createQuestionBankQuestion**
> CreateDarIntegration201Response createQuestionBankQuestion(createQuestionBankQuestionRequest)

Create a new system question bank question with FE-helpful input format

### Example

```typescript
import {
    QuestionBankApi,
    Configuration,
    CreateQuestionBankQuestionRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new QuestionBankApi(configuration);

let createQuestionBankQuestionRequest: CreateQuestionBankQuestionRequest; //QuestionBank definition

const { status, data } = await apiInstance.createQuestionBankQuestion(
    createQuestionBankQuestionRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createQuestionBankQuestionRequest** | **CreateQuestionBankQuestionRequest**| QuestionBank definition | |


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

# **deleteQuestionBankQuestion**
> DeleteApplications200Response deleteQuestionBankQuestion()

Delete a system question bank question

### Example

```typescript
import {
    QuestionBankApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new QuestionBankApi(configuration);

let id: number; //question bank question id (default to undefined)

const { status, data } = await apiInstance.deleteQuestionBankQuestion(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | question bank question id | defaults to undefined|


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

# **downloadQuestionBankQuestionFile**
> DeleteApplications200Response downloadQuestionBankQuestionFile()

Download a system question bank question

### Example

```typescript
import {
    QuestionBankApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new QuestionBankApi(configuration);

let id: number; //question bank question id (default to undefined)
let fileId: number; //file uuid (default to undefined)

const { status, data } = await apiInstance.downloadQuestionBankQuestionFile(
    id,
    fileId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | question bank question id | defaults to undefined|
| **fileId** | [**number**] | file uuid | defaults to undefined|


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

# **editQuestionBankQuestion**
> UpdateQuestionBankQuestion200Response editQuestionBankQuestion(editQuestionBankQuestionRequest)

Edit a system question bank question - use this for parents and children separately

### Example

```typescript
import {
    QuestionBankApi,
    Configuration,
    EditQuestionBankQuestionRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new QuestionBankApi(configuration);

let id: number; //question bank question id (default to undefined)
let editQuestionBankQuestionRequest: EditQuestionBankQuestionRequest; //QuestionBank definition

const { status, data } = await apiInstance.editQuestionBankQuestion(
    id,
    editQuestionBankQuestionRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **editQuestionBankQuestionRequest** | **EditQuestionBankQuestionRequest**| QuestionBank definition | |
| **id** | [**number**] | question bank question id | defaults to undefined|


### Return type

**UpdateQuestionBankQuestion200Response**

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

# **fetchArchivedQuestionBankQuestions**
> FetchQuestionBankQuestions200Response fetchArchivedQuestionBankQuestions()

List of archived question bank questions

### Example

```typescript
import {
    QuestionBankApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new QuestionBankApi(configuration);

let sectionId: number; //section id (optional) (default to undefined)
let isChild: number; //filter on is_child field (optional) (default to undefined)
let perPage: number; //per page (optional) (default to undefined)
let page: number; //page (optional) (default to undefined)

const { status, data } = await apiInstance.fetchArchivedQuestionBankQuestions(
    sectionId,
    isChild,
    perPage,
    page
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sectionId** | [**number**] | section id | (optional) defaults to undefined|
| **isChild** | [**number**] | filter on is_child field | (optional) defaults to undefined|
| **perPage** | [**number**] | per page | (optional) defaults to undefined|
| **page** | [**number**] | page | (optional) defaults to undefined|


### Return type

**FetchQuestionBankQuestions200Response**

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

# **fetchCustomQuestionBankQuestions**
> FetchCustomQuestionBankQuestions200Response fetchCustomQuestionBankQuestions()

List of custom question bank questions

### Example

```typescript
import {
    QuestionBankApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new QuestionBankApi(configuration);

let sectionId: number; //section id (optional) (default to undefined)
let isChild: number; //filter on is_child field (optional) (default to undefined)
let perPage: number; //per page (optional) (default to undefined)
let page: number; //page (optional) (default to undefined)

const { status, data } = await apiInstance.fetchCustomQuestionBankQuestions(
    sectionId,
    isChild,
    perPage,
    page
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sectionId** | [**number**] | section id | (optional) defaults to undefined|
| **isChild** | [**number**] | filter on is_child field | (optional) defaults to undefined|
| **perPage** | [**number**] | per page | (optional) defaults to undefined|
| **page** | [**number**] | page | (optional) defaults to undefined|


### Return type

**FetchCustomQuestionBankQuestions200Response**

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

# **fetchQuestionBankQuestion**
> FetchQuestionBankQuestion200Response fetchQuestionBankQuestion()

Return the latest question bank question version for the supplied question id, in an FE-friendly format

### Example

```typescript
import {
    QuestionBankApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new QuestionBankApi(configuration);

let id: number; //question bank question id (default to undefined)

const { status, data } = await apiInstance.fetchQuestionBankQuestion(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | question bank question id | defaults to undefined|


### Return type

**FetchQuestionBankQuestion200Response**

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

# **fetchQuestionBankQuestionVersion**
> FetchQuestionBankQuestionVersion200Response fetchQuestionBankQuestionVersion()

Return a single system question bank question version

### Example

```typescript
import {
    QuestionBankApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new QuestionBankApi(configuration);

let id: number; //question bank question version id (default to undefined)

const { status, data } = await apiInstance.fetchQuestionBankQuestionVersion(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | question bank question version id | defaults to undefined|


### Return type

**FetchQuestionBankQuestionVersion200Response**

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

# **fetchQuestionBankQuestions**
> FetchQuestionBankQuestions200Response fetchQuestionBankQuestions()

List of question bank questions

### Example

```typescript
import {
    QuestionBankApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new QuestionBankApi(configuration);

let sectionId: number; //section id (optional) (default to undefined)
let isChild: number; //filter on is_child field (optional) (default to undefined)
let perPage: number; //per page (optional) (default to undefined)
let page: number; //page (optional) (default to undefined)

const { status, data } = await apiInstance.fetchQuestionBankQuestions(
    sectionId,
    isChild,
    perPage,
    page
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sectionId** | [**number**] | section id | (optional) defaults to undefined|
| **isChild** | [**number**] | filter on is_child field | (optional) defaults to undefined|
| **perPage** | [**number**] | per page | (optional) defaults to undefined|
| **page** | [**number**] | page | (optional) defaults to undefined|


### Return type

**FetchQuestionBankQuestions200Response**

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

# **fetchStandardQuestionBankQuestions**
> FetchStandardQuestionBankQuestions200Response fetchStandardQuestionBankQuestions()

List of standard question bank questions

### Example

```typescript
import {
    QuestionBankApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new QuestionBankApi(configuration);

let sectionId: number; //section id (optional) (default to undefined)
let isChild: number; //filter on is_child field (optional) (default to undefined)
let perPage: number; //per page (optional) (default to undefined)
let page: number; //page (optional) (default to undefined)

const { status, data } = await apiInstance.fetchStandardQuestionBankQuestions(
    sectionId,
    isChild,
    perPage,
    page
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sectionId** | [**number**] | section id | (optional) defaults to undefined|
| **isChild** | [**number**] | filter on is_child field | (optional) defaults to undefined|
| **perPage** | [**number**] | per page | (optional) defaults to undefined|
| **page** | [**number**] | page | (optional) defaults to undefined|


### Return type

**FetchStandardQuestionBankQuestions200Response**

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

# **fetchTeamQuestionBankQuestionsBySection**
> FetchTeamQuestionBankQuestionsBySection200Response fetchTeamQuestionBankQuestionsBySection()

List of question bank questions by section

### Example

```typescript
import {
    QuestionBankApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new QuestionBankApi(configuration);

let teamId: number; //Team ID (default to undefined)
let sectionId: number; //section id (default to undefined)
let isChild: number; //filter on is_child field (optional) (default to undefined)

const { status, data } = await apiInstance.fetchTeamQuestionBankQuestionsBySection(
    teamId,
    sectionId,
    isChild
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **teamId** | [**number**] | Team ID | defaults to undefined|
| **sectionId** | [**number**] | section id | defaults to undefined|
| **isChild** | [**number**] | filter on is_child field | (optional) defaults to undefined|


### Return type

**FetchTeamQuestionBankQuestionsBySection200Response**

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

# **updateQuestionBankQuestion**
> UpdateQuestionBankQuestion200Response updateQuestionBankQuestion(updateQuestionBankQuestionRequest)

Update a system question bank question - children and their versions are updated through parents

### Example

```typescript
import {
    QuestionBankApi,
    Configuration,
    UpdateQuestionBankQuestionRequest
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new QuestionBankApi(configuration);

let id: number; //question bank question id (default to undefined)
let updateQuestionBankQuestionRequest: UpdateQuestionBankQuestionRequest; //QuestionBank definition

const { status, data } = await apiInstance.updateQuestionBankQuestion(
    id,
    updateQuestionBankQuestionRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateQuestionBankQuestionRequest** | **UpdateQuestionBankQuestionRequest**| QuestionBank definition | |
| **id** | [**number**] | question bank question id | defaults to undefined|


### Return type

**UpdateQuestionBankQuestion200Response**

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

# **updateQuestionBankQuestionStatus**
> UpdateQuestionBankQuestionStatus200Response updateQuestionBankQuestionStatus()

Lock, unlock, archive or unarchive a question bank question

### Example

```typescript
import {
    QuestionBankApi,
    Configuration
} from '@hdruk/gateway-api-sdk';

const configuration = new Configuration();
const apiInstance = new QuestionBankApi(configuration);

let id: number; //question bank question id (default to undefined)
let status: string; //lock or unlock (default to undefined)

const { status, data } = await apiInstance.updateQuestionBankQuestionStatus(
    id,
    status
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | question bank question id | defaults to undefined|
| **status** | [**string**] | lock or unlock | defaults to undefined|


### Return type

**UpdateQuestionBankQuestionStatus200Response**

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

