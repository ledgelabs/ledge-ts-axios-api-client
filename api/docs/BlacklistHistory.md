# BlacklistHistory


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**apiKeyId** | **string** |  | [default to undefined]
**action** | [**BlacklistAction**](BlacklistAction.md) |  | [default to undefined]
**severity** | [**BlacklistSeverity**](BlacklistSeverity.md) |  | [default to undefined]
**notes** | **string** |  | [default to undefined]
**userId** | **string** |  | [default to undefined]
**user** | [**User**](User.md) |  | [optional] [default to undefined]

## Example

```typescript
import { BlacklistHistory } from './api';

const instance: BlacklistHistory = {
    id,
    createdAt,
    updatedAt,
    apiKeyId,
    action,
    severity,
    notes,
    userId,
    user,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
