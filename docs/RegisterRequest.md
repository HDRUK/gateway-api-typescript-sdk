# RegisterRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **string** | Email address | [optional] [default to undefined]
**password** | **string** | Password (minimum 8 characters) | [optional] [default to undefined]
**firstname** | **string** | First name (optional) | [optional] [default to undefined]
**lastname** | **string** | Last name (optional) | [optional] [default to undefined]
**provider** | **string** | Optional. Set to \&#39;cruk\&#39; for CRUK registration only; otherwise ignored (service). | [optional] [default to undefined]

## Example

```typescript
import { RegisterRequest } from '@hdruk/gateway-api-sdk';

const instance: RegisterRequest = {
    email,
    password,
    firstname,
    lastname,
    provider,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
