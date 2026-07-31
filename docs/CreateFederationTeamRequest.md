# CreateFederationTeamRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**federation_type** | **string** |  | [optional] [default to undefined]
**auth_type** | **string** |  | [optional] [default to undefined]
**auth_secret_key** | **string** |  | [optional] [default to undefined]
**endpoint_baseurl** | **string** |  | [optional] [default to undefined]
**endpoint_datasets** | **string** |  | [optional] [default to undefined]
**endpoint_dataset** | **string** |  | [optional] [default to undefined]
**run_time_hour** | **number** |  | [optional] [default to undefined]
**enabled** | **boolean** |  | [optional] [default to undefined]
**notifications** | **Array&lt;Array&lt;any&gt;&gt;** |  | [optional] [default to undefined]
**tested** | **boolean** |  | [optional] [default to undefined]

## Example

```typescript
import { CreateFederationTeamRequest } from '@hdruk/gateway-api-sdk';

const instance: CreateFederationTeamRequest = {
    federation_type,
    auth_type,
    auth_secret_key,
    endpoint_baseurl,
    endpoint_datasets,
    endpoint_dataset,
    run_time_hour,
    enabled,
    notifications,
    tested,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
