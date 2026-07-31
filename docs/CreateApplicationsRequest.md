# CreateApplicationsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [optional] [default to undefined]
**image_link** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**team_id** | **number** |  | [optional] [default to undefined]
**user_id** | **number** |  | [optional] [default to undefined]
**enabled** | **boolean** |  | [optional] [default to undefined]
**permissions** | **Array&lt;any&gt;** |  | [optional] [default to undefined]
**notifications** | **Array&lt;any&gt;** |  | [optional] [default to undefined]

## Example

```typescript
import { CreateApplicationsRequest } from '@hdruk/gateway-api-sdk';

const instance: CreateApplicationsRequest = {
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
