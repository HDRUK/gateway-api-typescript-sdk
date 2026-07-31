# DataAccessApplication

A Data Access Application (DAR) record managed by the Gateway

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [default to undefined]
**applicant_id** | **number** |  | [optional] [default to undefined]
**project_title** | **string** |  | [optional] [default to undefined]
**project_id** | **string** |  | [optional] [default to undefined]
**application_type** | **string** |  | [optional] [default to undefined]
**submission_status** | **string** |  | [optional] [default to undefined]
**approval_status** | **string** |  | [optional] [default to undefined]
**is_joint** | **boolean** |  | [optional] [default to undefined]
**status_review_id** | **number** |  | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]
**deleted_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { DataAccessApplication } from '@hdruk/gateway-api-sdk';

const instance: DataAccessApplication = {
    id,
    applicant_id,
    project_title,
    project_id,
    application_type,
    submission_status,
    approval_status,
    is_joint,
    status_review_id,
    created_at,
    updated_at,
    deleted_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
