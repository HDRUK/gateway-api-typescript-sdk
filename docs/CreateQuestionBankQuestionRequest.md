# CreateQuestionBankQuestionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**section_id** | **number** |  | [default to undefined]
**user_id** | **number** |  | [optional] [default to undefined]
**team_ids** | **Array&lt;number&gt;** |  | [optional] [default to undefined]
**locked** | **boolean** |  | [optional] [default to undefined]
**archived** | **boolean** |  | [optional] [default to undefined]
**required** | **boolean** |  | [optional] [default to undefined]
**force_required** | **boolean** |  | [default to undefined]
**allow_guidance_override** | **boolean** |  | [default to undefined]
**_default** | **boolean** |  | [optional] [default to undefined]
**guidance** | **string** |  | [default to undefined]
**title** | **string** |  | [default to undefined]
**field** | **Array&lt;object&gt;** |  | [default to undefined]
**component** | **string** |  | [default to undefined]
**validations** | **Array&lt;object&gt;** |  | [default to undefined]
**_options** | [**Array&lt;CreateQuestionBankQuestionRequestOptionsInner&gt;**](CreateQuestionBankQuestionRequestOptionsInner.md) |  | [default to undefined]
**is_child** | **boolean** |  | [optional] [default to undefined]
**question_type** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { CreateQuestionBankQuestionRequest } from '@hdruk/gateway-api-sdk';

const instance: CreateQuestionBankQuestionRequest = {
    section_id,
    user_id,
    team_ids,
    locked,
    archived,
    required,
    force_required,
    allow_guidance_override,
    _default,
    guidance,
    title,
    field,
    component,
    validations,
    _options,
    is_child,
    question_type,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
