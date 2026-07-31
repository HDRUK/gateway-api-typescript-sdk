# LoginRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **string** | Email address | [optional] [default to undefined]
**password** | **string** | Password | [optional] [default to undefined]
**provider** | **string** | Optional. Set to \&#39;cruk\&#39; for CRUK login only; otherwise ignored (service). | [optional] [default to undefined]

## Example

```typescript
import { LoginRequest } from '@hdruk/gateway-api-sdk';

const instance: LoginRequest = {
    email,
    password,
    provider,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
