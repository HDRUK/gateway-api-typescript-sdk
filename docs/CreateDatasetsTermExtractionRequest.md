# CreateDatasetsTermExtractionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**partial** | **boolean** | Flag to determine if term extraction should be partial (true) or full (false) | [optional] [default to true]
**minId** | **number** | Minimum dataset ID to include in the term extraction | [optional] [default to 1]
**maxId** | **number** | Maximum dataset ID to include in the term extraction. Defaults to the maximum dataset ID available. | [optional] [default to undefined]
**indexElastic** | **boolean** | Flag to determine if data should be indexed in Elasticsearch | [optional] [default to true]

## Example

```typescript
import { CreateDatasetsTermExtractionRequest } from '@hdruk/gateway-api-sdk';

const instance: CreateDatasetsTermExtractionRequest = {
    partial,
    minId,
    maxId,
    indexElastic,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
