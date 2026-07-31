# UpdateToolsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [optional] [default to undefined]
**url** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**license** | **number** |  | [optional] [default to undefined]
**tech_stack** | **string** |  | [optional] [default to undefined]
**category_id** | **number** |  | [optional] [default to undefined]
**user_id** | **number** |  | [optional] [default to undefined]
**team_id** | **number** |  | [optional] [default to undefined]
**tags** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**dataset** | [**Array&lt;CreateToolsIntegrationsRequestDatasetInner&gt;**](CreateToolsIntegrationsRequestDatasetInner.md) |  | [optional] [default to undefined]
**enabled** | **number** |  | [optional] [default to undefined]
**programming_language** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**programming_package** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**type_category** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**associated_authors** | **string** |  | [optional] [default to undefined]
**contact_address** | **string** |  | [optional] [default to undefined]
**publications** | [**Array&lt;CreateToolsIntegrationsRequestPublicationsInner&gt;**](CreateToolsIntegrationsRequestPublicationsInner.md) |  | [optional] [default to undefined]
**durs** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**collections** | [**Array&lt;CreateToolsRequestCollectionsInner&gt;**](CreateToolsRequestCollectionsInner.md) |  | [optional] [default to undefined]
**any_dataset** | **boolean** |  | [optional] [default to undefined]
**status** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { UpdateToolsRequest } from '@hdruk/gateway-api-sdk';

const instance: UpdateToolsRequest = {
    name,
    url,
    description,
    license,
    tech_stack,
    category_id,
    user_id,
    team_id,
    tags,
    dataset,
    enabled,
    programming_language,
    programming_package,
    type_category,
    associated_authors,
    contact_address,
    publications,
    durs,
    collections,
    any_dataset,
    status,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
