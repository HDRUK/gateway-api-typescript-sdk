# User

A registered Gateway user

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**firstname** | **string** |  | [optional] [default to undefined]
**lastname** | **string** |  | [optional] [default to undefined]
**email** | **string** |  | [optional] [default to undefined]
**secondary_email** | **string** |  | [optional] [default to undefined]
**preferred_email** | **string** |  | [optional] [default to undefined]
**provider** | **string** |  | [optional] [default to undefined]
**sector_id** | **number** |  | [optional] [default to undefined]
**organisation** | **string** |  | [optional] [default to undefined]
**bio** | **string** |  | [optional] [default to undefined]
**domain** | **string** |  | [optional] [default to undefined]
**link** | **string** |  | [optional] [default to undefined]
**orcid** | **string** |  | [optional] [default to undefined]
**contact_feedback** | **boolean** |  | [optional] [default to undefined]
**contact_news** | **boolean** |  | [optional] [default to undefined]
**is_admin** | **boolean** |  | [optional] [default to undefined]
**terms** | **boolean** |  | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { User } from '@hdruk/gateway-api-sdk';

const instance: User = {
    id,
    name,
    firstname,
    lastname,
    email,
    secondary_email,
    preferred_email,
    provider,
    sector_id,
    organisation,
    bio,
    domain,
    link,
    orcid,
    contact_feedback,
    contact_news,
    is_admin,
    terms,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
