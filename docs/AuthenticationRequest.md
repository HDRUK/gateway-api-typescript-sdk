# AuthenticationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **string** | Email | [optional] [default to undefined]
**password** | **string** | Password | [optional] [default to undefined]
**provider** | **string** | Optional. Set to \&#39;cruk\&#39; for CRUK auth only; otherwise ignored (service). | [optional] [default to undefined]

## Example

```typescript
import { AuthenticationRequest } from '@hdruk/gateway-api-sdk';

const instance: AuthenticationRequest = {
    email,
    password,
    provider,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
