# GetFederationHistory200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**job_uuid** | **string** |  | [optional] [default to undefined]
**started_at** | **string** |  | [optional] [default to undefined]
**finished_at** | **string** |  | [optional] [default to undefined]
**status** | **string** |  | [optional] [default to undefined]
**message** | **string** |  | [optional] [default to undefined]
**failed_datasets** | [**Array&lt;GetFederationHistory200ResponseDataInnerFailedDatasetsInner&gt;**](GetFederationHistory200ResponseDataInnerFailedDatasetsInner.md) |  | [optional] [default to undefined]

## Example

```typescript
import { GetFederationHistory200ResponseDataInner } from '@hdruk/gateway-api-sdk';

const instance: GetFederationHistory200ResponseDataInner = {
    job_uuid,
    started_at,
    finished_at,
    status,
    message,
    failed_datasets,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
