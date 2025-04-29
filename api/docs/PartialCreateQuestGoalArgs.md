# PartialCreateQuestGoalArgs

Make all properties in T optional

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | [**QuestType**](QuestType.md) |  | [optional] [default to undefined]
**title** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**target** | **number** |  | [optional] [default to undefined]
**activity** | [**ActivityType**](ActivityType.md) |  | [optional] [default to undefined]
**objectId** | **string** |  | [optional] [default to undefined]
**openUrl** | **string** |  | [optional] [default to undefined]
**bannerUrl** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { PartialCreateQuestGoalArgs } from './api';

const instance: PartialCreateQuestGoalArgs = {
    type,
    title,
    description,
    target,
    activity,
    objectId,
    openUrl,
    bannerUrl,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
