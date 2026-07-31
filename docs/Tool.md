# Tool

A software tool or model associated with datasets in the Gateway

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**url** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**results_insights** | **string** |  | [optional] [default to undefined]
**license** | **number** | Foreign key to licenses table | [optional] [default to undefined]
**tech_stack** | **string** |  | [optional] [default to undefined]
**category_id** | **number** |  | [optional] [default to undefined]
**user_id** | **number** |  | [optional] [default to undefined]
**enabled** | **boolean** |  | [optional] [default to undefined]
**associated_authors** | **string** |  | [optional] [default to undefined]
**contact_address** | **string** |  | [optional] [default to undefined]
**any_dataset** | **boolean** |  | [optional] [default to undefined]
**status** | **string** |  | [optional] [default to undefined]
**team_id** | **number** |  | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { Tool } from '@hdruk/gateway-api-sdk';

const instance: Tool = {
    id,
    name,
    url,
    description,
    results_insights,
    license,
    tech_stack,
    category_id,
    user_id,
    enabled,
    associated_authors,
    contact_address,
    any_dataset,
    status,
    team_id,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
