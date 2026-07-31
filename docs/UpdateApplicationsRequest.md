# UpdateApplicationsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [default to undefined]
**image_link** | **string** |  | [default to undefined]
**description** | **string** |  | [default to undefined]
**team_id** | **number** |  | [default to undefined]
**user_id** | **number** |  | [default to undefined]
**enabled** | **boolean** |  | [default to undefined]
**permissions** | **Array&lt;any&gt;** |  | [default to undefined]
**notifications** | **Array&lt;any&gt;** |  | [optional] [default to undefined]

## Example

```typescript
import { UpdateApplicationsRequest } from '@hdruk/gateway-api-sdk';

const instance: UpdateApplicationsRequest = {
    name,
    image_link,
    description,
    team_id,
    user_id,
    enabled,
    permissions,
    notifications,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
