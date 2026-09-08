# UpdatePublicationsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**paper_title** | **string** |  | [optional] [default to undefined]
**authors** | **string** |  | [optional] [default to undefined]
**year_of_publication** | **string** |  | [optional] [default to undefined]
**paper_doi** | **string** |  | [optional] [default to undefined]
**publication_type** | **string** |  | [optional] [default to undefined]
**journal_name** | **string** |  | [optional] [default to undefined]
**_abstract** | **string** |  | [optional] [default to undefined]
**url** | **string** |  | [optional] [default to undefined]
**status** | **string** |  | [optional] [default to undefined]
**datasets** | [**Array&lt;CreatePublicationsRequestDatasetsInner&gt;**](CreatePublicationsRequestDatasetsInner.md) |  | [optional] [default to undefined]
**tools** | [**Array&lt;CreatePublicationsRequestToolsInner&gt;**](CreatePublicationsRequestToolsInner.md) |  | [optional] [default to undefined]

## Example

```typescript
import { UpdatePublicationsRequest } from '@hdruk/gateway-api-sdk';

const instance: UpdatePublicationsRequest = {
    paper_title,
    authors,
    year_of_publication,
    paper_doi,
    publication_type,
    journal_name,
    _abstract,
    url,
    status,
    datasets,
    tools,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
