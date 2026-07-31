# SavedSearch

A user\'s saved search definition

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [default to undefined]
**user_id** | **number** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**search_term** | **string** |  | [optional] [default to undefined]
**search_endpoint** | **string** |  | [optional] [default to undefined]
**sort_order** | **string** |  | [optional] [default to undefined]
**enabled** | **boolean** |  | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]
**deleted_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { SavedSearch } from '@hdruk/gateway-api-sdk';

const instance: SavedSearch = {
    id,
    user_id,
    name,
    search_term,
    search_endpoint,
    sort_order,
    enabled,
    created_at,
    updated_at,
    deleted_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
