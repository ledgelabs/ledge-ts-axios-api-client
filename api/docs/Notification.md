# Notification


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**type** | [**NotificationType**](NotificationType.md) |  | [default to undefined]
**objectId** | **string** |  | [default to undefined]
**seen** | **boolean** |  | [default to undefined]
**title** | **string** |  | [default to undefined]
**subtitle** | **string** |  | [default to undefined]
**description** | **string** |  | [default to undefined]
**bannerUrl** | **string** |  | [default to undefined]
**userId** | **string** |  | [default to undefined]
**user** | [**User**](User.md) |  | [optional] [default to undefined]

## Example

```typescript
import { Notification } from './api';

const instance: Notification = {
    id,
    createdAt,
    updatedAt,
    type,
    objectId,
    seen,
    title,
    subtitle,
    description,
    bannerUrl,
    userId,
    user,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
