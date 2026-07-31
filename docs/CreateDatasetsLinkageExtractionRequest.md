# CreateDatasetsLinkageExtractionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**minId** | **number** | Minimum dataset ID to include in the term extraction | [optional] [default to 1]
**maxId** | **number** | Maximum dataset ID to include in the term extraction. Defaults to the maximum dataset ID available. | [optional] [default to undefined]

## Example

```typescript
import { CreateDatasetsLinkageExtractionRequest } from '@hdruk/gateway-api-sdk';

const instance: CreateDatasetsLinkageExtractionRequest = {
    minId,
    maxId,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
