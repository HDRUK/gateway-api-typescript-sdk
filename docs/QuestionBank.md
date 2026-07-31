# QuestionBank

A question bank question record managed by the Gateway

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [default to undefined]
**section_id** | **number** |  | [optional] [default to undefined]
**user_id** | **number** |  | [optional] [default to undefined]
**locked** | **boolean** |  | [optional] [default to undefined]
**archived** | **boolean** |  | [optional] [default to undefined]
**archived_date** | **string** |  | [optional] [default to undefined]
**force_required** | **boolean** |  | [optional] [default to undefined]
**allow_guidance_override** | **boolean** |  | [optional] [default to undefined]
**is_child** | **boolean** |  | [optional] [default to undefined]
**question_type** | **string** |  | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { QuestionBank } from '@hdruk/gateway-api-sdk';

const instance: QuestionBank = {
    id,
    section_id,
    user_id,
    locked,
    archived,
    archived_date,
    force_required,
    allow_guidance_override,
    is_child,
    question_type,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
