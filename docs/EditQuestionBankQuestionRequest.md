# EditQuestionBankQuestionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**section_id** | **number** |  | [optional] [default to undefined]
**user_id** | **number** |  | [optional] [default to undefined]
**team_ids** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**locked** | **boolean** |  | [optional] [default to undefined]
**archived** | **boolean** |  | [optional] [default to undefined]
**force_required** | **boolean** |  | [optional] [default to undefined]
**allow_guidance_override** | **boolean** |  | [optional] [default to undefined]
**question_type** | **string** |  | [optional] [default to undefined]
**_default** | **boolean** |  | [optional] [default to undefined]
**guidance** | **string** |  | [optional] [default to undefined]
**title** | **string** |  | [optional] [default to undefined]
**field** | **Array&lt;object&gt;** |  | [optional] [default to undefined]

## Example

```typescript
import { EditQuestionBankQuestionRequest } from '@hdruk/gateway-api-sdk';

const instance: EditQuestionBankQuestionRequest = {
    section_id,
    user_id,
    team_ids,
    locked,
    archived,
    force_required,
    allow_guidance_override,
    question_type,
    _default,
    guidance,
    title,
    field,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
