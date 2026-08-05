# EditCollectionsV2Request


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
**collaborators** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**_public** | **boolean** |  | [optional] [default to undefined]
**status** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { EditCollectionsV2Request } from '@hdruk/gateway-api-sdk';

const instance: EditCollectionsV2Request = {
    name,
    description,
    image_link,
    enabled,
    keywords,
    datasets,
    dur,
    publications,
    collaborators,
    _public,
    status,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
