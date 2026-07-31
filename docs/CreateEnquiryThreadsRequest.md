# CreateEnquiryThreadsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **number** |  | [default to undefined]
**project_title** | **string** |  | [default to undefined]
**is_dar_dialogue** | **boolean** |  | [optional] [default to undefined]
**is_dar_status** | **boolean** |  | [optional] [default to undefined]
**is_feasibility_enquiry** | **boolean** |  | [optional] [default to undefined]
**is_general_enquiry** | **boolean** |  | [optional] [default to undefined]
**is_dar_review** | **boolean** |  | [optional] [default to undefined]
**enabled** | **boolean** |  | [optional] [default to undefined]

## Example

```typescript
import { CreateEnquiryThreadsRequest } from '@hdruk/gateway-api-sdk';

const instance: CreateEnquiryThreadsRequest = {
    user_id,
    project_title,
    is_dar_dialogue,
    is_dar_status,
    is_feasibility_enquiry,
    is_general_enquiry,
    is_dar_review,
    enabled,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
