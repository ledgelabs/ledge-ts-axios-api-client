# Quest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**title** | **string** |  | [default to undefined]
**description** | **string** |  | [default to undefined]
**type** | [**QuestType**](QuestType.md) |  | [default to undefined]
**gameId** | **string** |  | [default to undefined]
**game** | [**Game**](Game.md) |  | [optional] [default to undefined]
**eventId** | **string** |  | [default to undefined]
**event** | [**Event**](Event.md) |  | [optional] [default to undefined]
**goals** | [**Array&lt;Goal&gt;**](Goal.md) |  | [optional] [default to undefined]
**schedules** | [**Array&lt;QuestSchedule&gt;**](QuestSchedule.md) |  | [optional] [default to undefined]

## Example

```typescript
import { Quest } from './api';

const instance: Quest = {
    id,
    createdAt,
    updatedAt,
    title,
    description,
    type,
    gameId,
    game,
    eventId,
    event,
    goals,
    schedules,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
