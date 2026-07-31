# Widget

A widget record managed by the Gateway

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [default to undefined]
**team_id** | **number** |  | [optional] [default to undefined]
**data_custodian_entities_ids** | **string** |  | [optional] [default to undefined]
**included_datasets** | **string** |  | [optional] [default to undefined]
**included_data_uses** | **string** |  | [optional] [default to undefined]
**included_scripts** | **string** |  | [optional] [default to undefined]
**included_collections** | **string** |  | [optional] [default to undefined]
**include_search_bar** | **boolean** |  | [optional] [default to undefined]
**include_cohort_link** | **boolean** |  | [optional] [default to undefined]
**size_width** | **number** |  | [optional] [default to undefined]
**size_height** | **number** |  | [optional] [default to undefined]
**unit** | **string** |  | [optional] [default to undefined]
**keep_proportions** | **boolean** |  | [optional] [default to undefined]
**widget_name** | **string** |  | [optional] [default to undefined]
**permitted_domains** | **string** |  | [optional] [default to undefined]
**branding_primary** | **string** |  | [optional] [default to undefined]
**branding_secondary** | **string** |  | [optional] [default to undefined]
**branding_neutral** | **string** |  | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { Widget } from '@hdruk/gateway-api-sdk';

const instance: Widget = {
    id,
    team_id,
    data_custodian_entities_ids,
    included_datasets,
    included_data_uses,
    included_scripts,
    included_collections,
    include_search_bar,
    include_cohort_link,
    size_width,
    size_height,
    unit,
    keep_proportions,
    widget_name,
    permitted_domains,
    branding_primary,
    branding_secondary,
    branding_neutral,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
