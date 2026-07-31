# Notification

A notification preference/subscription record

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [default to undefined]
**user_id** | **number** |  | [optional] [default to undefined]
**notification_type** | **string** |  | [optional] [default to undefined]
**message** | **string** |  | [optional] [default to undefined]
**opt_in** | **boolean** |  | [optional] [default to undefined]
**enabled** | **boolean** |  | [optional] [default to undefined]
**email** | **string** |  | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]
**deleted_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { Notification } from '@hdruk/gateway-api-sdk';

const instance: Notification = {
    id,
    user_id,
    notification_type,
    message,
    opt_in,
    enabled,
    email,
    created_at,
    updated_at,
    deleted_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
