# FetchTeamDarApplicationHeader200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]
**deleted_at** | **string** |  | [optional] [default to undefined]
**applicant_id** | **number** |  | [optional] [default to undefined]
**project_title** | **string** |  | [optional] [default to undefined]
**application_type** | **string** |  | [optional] [default to undefined]
**project_id** | **number** |  | [optional] [default to undefined]
**is_joint** | **boolean** |  | [optional] [default to undefined]
**approval_status** | **string** |  | [optional] [default to undefined]
**submission_status** | **string** |  | [optional] [default to undefined]
**status_review_id** | **number** |  | [optional] [default to undefined]
**days_since_submission** | **number** |  | [optional] [default to undefined]
**primary_applicant** | [**Array&lt;FetchTeamDarApplicationHeader200ResponseDataPrimaryApplicantInner&gt;**](FetchTeamDarApplicationHeader200ResponseDataPrimaryApplicantInner.md) |  | [optional] [default to undefined]
**datasets** | [**Array&lt;FetchTeamDarApplicationHeader200ResponseDataDatasetsInner&gt;**](FetchTeamDarApplicationHeader200ResponseDataDatasetsInner.md) |  | [optional] [default to undefined]
**teams** | [**Array&lt;FetchTeamDarApplicationHeader200ResponseDataTeamsInner&gt;**](FetchTeamDarApplicationHeader200ResponseDataTeamsInner.md) |  | [optional] [default to undefined]

## Example

```typescript
import { FetchTeamDarApplicationHeader200ResponseData } from '@hdruk/gateway-api-sdk';

const instance: FetchTeamDarApplicationHeader200ResponseData = {
    id,
    created_at,
    updated_at,
    deleted_at,
    applicant_id,
    project_title,
    application_type,
    project_id,
    is_joint,
    approval_status,
    submission_status,
    status_review_id,
    days_since_submission,
    primary_applicant,
    datasets,
    teams,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
