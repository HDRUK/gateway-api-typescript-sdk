# CreateDarTemplateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**team_id** | **number** |  | [default to undefined]
**user_id** | **number** |  | [optional] [default to undefined]
**published** | **boolean** |  | [optional] [default to undefined]
**locked** | **boolean** |  | [optional] [default to undefined]
**questions** | [**Array&lt;CreateDarTemplateRequestQuestionsInner&gt;**](CreateDarTemplateRequestQuestionsInner.md) |  | [optional] [default to undefined]

## Example

```typescript
import { CreateDarTemplateRequest } from '@hdruk/gateway-api-sdk';

const instance: CreateDarTemplateRequest = {
    team_id,
    user_id,
    published,
    locked,
    questions,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
