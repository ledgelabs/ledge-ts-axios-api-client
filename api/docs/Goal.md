# Goal


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**title** | **string** |  | [default to undefined]
**target** | **number** |  | [default to undefined]
**activity** | [**ActivityType**](ActivityType.md) |  | [default to undefined]
**description** | **string** |  | [default to undefined]
**instructions** | **string** |  | [default to undefined]
**bannerUrl** | **string** |  | [default to undefined]
**objectId** | **string** |  | [default to undefined]
**openUrl** | **string** |  | [default to undefined]
**questId** | **string** |  | [default to undefined]
**quest** | [**Quest**](Quest.md) |  | [optional] [default to undefined]
**goalAttributes** | [**Array&lt;GoalAttribute&gt;**](GoalAttribute.md) |  | [optional] [default to undefined]
**goalProducts** | [**Array&lt;GoalProduct&gt;**](GoalProduct.md) |  | [optional] [default to undefined]

## Example

```typescript
import { Goal } from './api';

const instance: Goal = {
    id,
    createdAt,
    updatedAt,
    title,
    target,
    activity,
    description,
    instructions,
    bannerUrl,
    objectId,
    openUrl,
    questId,
    quest,
    goalAttributes,
    goalProducts,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
