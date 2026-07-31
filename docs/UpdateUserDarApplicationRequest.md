# UpdateUserDarApplicationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**applicant_id** | **number** |  | [default to undefined]
**submission_status** | **string** |  | [default to undefined]
**project_title** | **string** |  | [optional] [default to undefined]
**approval_status** | **string** |  | [default to undefined]
**team_ids** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**answers** | [**Array&lt;UpdateUserDarApplicationRequestAnswersInner&gt;**](UpdateUserDarApplicationRequestAnswersInner.md) |  | [optional] [default to undefined]

## Example

```typescript
import { UpdateUserDarApplicationRequest } from '@hdruk/gateway-api-sdk';

const instance: UpdateUserDarApplicationRequest = {
    applicant_id,
    submission_status,
    project_title,
    approval_status,
    team_ids,
    answers,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
