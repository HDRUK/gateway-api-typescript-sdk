# UpdateSavedSearchesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [default to undefined]
**search_endpoint** | **string** |  | [optional] [default to undefined]
**filters** | [**Array&lt;CreateSavedSearchesRequestFiltersInner&gt;**](CreateSavedSearchesRequestFiltersInner.md) |  | [optional] [default to undefined]
**enabled** | **string** |  | [default to undefined]

## Example

```typescript
import { UpdateSavedSearchesRequest } from '@hdruk/gateway-api-sdk';

const instance: UpdateSavedSearchesRequest = {
    name,
    search_endpoint,
    filters,
    enabled,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
