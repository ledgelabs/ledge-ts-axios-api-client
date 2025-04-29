# UserConnection


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**email** | **string** |  | [default to undefined]
**nickname** | **string** |  | [default to undefined]
**socialConnectionType** | [**ConnectionType**](ConnectionType.md) |  | [default to undefined]
**sub** | **string** |  | [default to undefined]
**userId** | **string** |  | [default to undefined]
**user** | [**User**](User.md) |  | [optional] [default to undefined]

## Example

```typescript
import { UserConnection } from './api';

const instance: UserConnection = {
    id,
    createdAt,
    updatedAt,
    email,
    nickname,
    socialConnectionType,
    sub,
    userId,
    user,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
