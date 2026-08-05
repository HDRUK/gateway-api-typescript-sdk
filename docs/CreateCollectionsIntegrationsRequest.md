# CreateCollectionsIntegrationsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**image_link** | **string** |  | [optional] [default to undefined]
**enabled** | **boolean** |  | [optional] [default to undefined]
**keywords** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**datasets** | [**Array&lt;CreateCollectionsIntegrationsRequestDatasetsInner&gt;**](CreateCollectionsIntegrationsRequestDatasetsInner.md) |  | [optional] [default to undefined]
**dur** | [**Array&lt;CreateCollectionsIntegrationsRequestDatasetsInner&gt;**](CreateCollectionsIntegrationsRequestDatasetsInner.md) |  | [optional] [default to undefined]
**publications** | [**Array&lt;CreateCollectionsIntegrationsRequestDatasetsInner&gt;**](CreateCollectionsIntegrationsRequestDatasetsInner.md) |  | [optional] [default to undefined]
**_public** | **boolean** |  | [optional] [default to undefined]

## Example

```typescript
import { CreateCollectionsIntegrationsRequest } from '@hdruk/gateway-api-sdk';

const instance: CreateCollectionsIntegrationsRequest = {
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
