# Team

A data custodian team that owns datasets and manages data access

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**enabled** | **boolean** |  | [optional] [default to undefined]
**allows_messaging** | **boolean** |  | [optional] [default to undefined]
**workflow_enabled** | **boolean** |  | [optional] [default to undefined]
**access_requests_management** | **boolean** |  | [optional] [default to undefined]
**uses_5_safes** | **boolean** |  | [optional] [default to undefined]
**is_admin** | **boolean** |  | [optional] [default to undefined]
**member_of** | **string** |  | [optional] [default to undefined]
**contact_point** | **string** |  | [optional] [default to undefined]
**notification_status** | **boolean** |  | [optional] [default to undefined]
**is_question_bank** | **boolean** |  | [optional] [default to undefined]
**team_logo** | **string** |  | [optional] [default to undefined]
**introduction** | **string** |  | [optional] [default to undefined]
**dar_modal_content** | **string** |  | [optional] [default to undefined]
**dar_modal_header** | **string** |  | [optional] [default to undefined]
**dar_modal_footer** | **string** |  | [optional] [default to undefined]
**service** | **string** |  | [optional] [default to undefined]
**is_dar** | **boolean** |  | [optional] [default to undefined]
**pid** | **string** | Public identifier, cast to string | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { Team } from '@hdruk/gateway-api-sdk';

const instance: Team = {
    id,
    name,
    enabled,
    allows_messaging,
    workflow_enabled,
    access_requests_management,
    uses_5_safes,
    is_admin,
    member_of,
    contact_point,
    notification_status,
    is_question_bank,
    team_logo,
    introduction,
    dar_modal_content,
    dar_modal_header,
    dar_modal_footer,
    service,
    is_dar,
    pid,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
