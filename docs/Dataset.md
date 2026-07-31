# Dataset

A dataset record managed by the Gateway

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [default to undefined]
**user_id** | **number** |  | [optional] [default to undefined]
**team_id** | **number** |  | [optional] [default to undefined]
**pid** | **string** |  | [optional] [default to undefined]
**datasetid** | **string** |  | [optional] [default to undefined]
**version** | **number** |  | [optional] [default to undefined]
**status** | **string** |  | [optional] [default to undefined]
**create_origin** | **string** |  | [optional] [default to undefined]
**is_cohort_discovery** | **boolean** |  | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { Dataset } from '@hdruk/gateway-api-sdk';

const instance: Dataset = {
    id,
    user_id,
    team_id,
    pid,
    datasetid,
    version,
    status,
    create_origin,
    is_cohort_discovery,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
