# UpdateWidgetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**widget_name** | **string** |  | [optional] [default to undefined]
**size_width** | **number** |  | [optional] [default to undefined]
**size_height** | **number** |  | [optional] [default to undefined]
**unit** | **string** |  | [optional] [default to undefined]
**include_search_bar** | **boolean** |  | [optional] [default to undefined]
**include_cohort_link** | **boolean** |  | [optional] [default to undefined]
**keep_proportions** | **boolean** |  | [optional] [default to undefined]
**permitted_domains** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**included_datasets** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**included_data_uses** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**data_custodian_entities_ids** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**included_scripts** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**included_collections** | **Array&lt;number&gt;** |  | [optional] [default to undefined]

## Example

```typescript
import { UpdateWidgetRequest } from '@hdruk/gateway-api-sdk';

const instance: UpdateWidgetRequest = {
    widget_name,
    size_width,
    size_height,
    unit,
    include_search_bar,
    include_cohort_link,
    keep_proportions,
    permitted_domains,
    included_datasets,
    included_data_uses,
    data_custodian_entities_ids,
    included_scripts,
    included_collections,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
