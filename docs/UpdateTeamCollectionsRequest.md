# UpdateTeamCollectionsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**image_link** | **string** |  | [optional] [default to undefined]
**enabled** | **boolean** |  | [optional] [default to undefined]
**keywords** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**datasets** | [**Array&lt;CreateTeamCollectionsRequestDatasetsInner&gt;**](CreateTeamCollectionsRequestDatasetsInner.md) |  | [optional] [default to undefined]
**dur** | [**Array&lt;CreateTeamCollectionsRequestDatasetsInner&gt;**](CreateTeamCollectionsRequestDatasetsInner.md) |  | [optional] [default to undefined]
**publications** | [**Array&lt;CreateTeamCollectionsRequestDatasetsInner&gt;**](CreateTeamCollectionsRequestDatasetsInner.md) |  | [optional] [default to undefined]
**_public** | **boolean** |  | [optional] [default to undefined]

## Example

```typescript
import { UpdateTeamCollectionsRequest } from '@hdruk/gateway-api-sdk';

const instance: UpdateTeamCollectionsRequest = {
    name,
    description,
    image_link,
    enabled,
    keywords,
    datasets,
    dur,
    publications,
    _public,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
