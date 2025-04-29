# QuestSchedule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**startTime** | **string** |  | [default to undefined]
**endTime** | **string** |  | [default to undefined]
**recurring** | **boolean** |  | [default to undefined]
**processed** | **boolean** |  | [default to undefined]
**questId** | **string** |  | [default to undefined]
**quest** | [**Quest**](Quest.md) |  | [optional] [default to undefined]
**progress** | [**Array&lt;Progress&gt;**](Progress.md) |  | [optional] [default to undefined]

## Example

```typescript
import { QuestSchedule } from './api';

const instance: QuestSchedule = {
    id,
    createdAt,
    updatedAt,
    startTime,
    endTime,
    recurring,
    processed,
    questId,
    quest,
    progress,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
