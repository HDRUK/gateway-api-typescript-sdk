# DatasetVersion

A versioned snapshot of dataset metadata in GWDM format

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [default to undefined]
**dataset_id** | **number** |  | [optional] [default to undefined]
**version** | **number** |  | [optional] [default to undefined]
**title** | **string** |  | [optional] [default to undefined]
**short_title** | **string** |  | [optional] [default to undefined]
**metadata** | **object** | Full GWDM-format metadata document for this version | [optional] [default to undefined]
**patch** | **Array&lt;object&gt;** | RFC 6902 JSON Patch array used to reconstruct this version from the previous snapshot. Null for full snapshots (v1 and every 10th version). | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { DatasetVersion } from '@hdruk/gateway-api-sdk';

const instance: DatasetVersion = {
    id,
    dataset_id,
    version,
    title,
    short_title,
    metadata,
    patch,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
