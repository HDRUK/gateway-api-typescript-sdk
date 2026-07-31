# UpdateToolsIntegrationsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [optional] [default to undefined]
**url** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**license** | **string** |  | [optional] [default to undefined]
**tech_stack** | **string** |  | [optional] [default to undefined]
**category_id** | **number** |  | [optional] [default to undefined]
**user_id** | **number** |  | [optional] [default to undefined]
**tags** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**programming_language** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**programming_package** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**dataset** | [**Array&lt;CreateToolsIntegrationsRequestDatasetInner&gt;**](CreateToolsIntegrationsRequestDatasetInner.md) |  | [optional] [default to undefined]
**type_category** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**enabled** | **number** |  | [optional] [default to undefined]
**publications** | [**Array&lt;CreateToolsIntegrationsRequestPublicationsInner&gt;**](CreateToolsIntegrationsRequestPublicationsInner.md) |  | [optional] [default to undefined]

## Example

```typescript
import { UpdateToolsIntegrationsRequest } from '@hdruk/gateway-api-sdk';

const instance: UpdateToolsIntegrationsRequest = {
    name,
    url,
    description,
    license,
    tech_stack,
    category_id,
    user_id,
    tags,
    programming_language,
    programming_package,
    dataset,
    type_category,
    enabled,
    publications,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
