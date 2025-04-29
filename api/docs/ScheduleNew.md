# ScheduleNew


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**startTime** | **string** |  | [default to undefined]
**endTime** | **string** |  | [default to undefined]
**type** | [**ScheduleType**](ScheduleType.md) |  | [default to undefined]
**objectId** | **string** |  | [default to undefined]
**frequency** | [**Frequency**](Frequency.md) |  | [default to undefined]
**interval** | **number** |  | [default to undefined]
**daysOfWeek** | **string** |  | [default to undefined]
**dayOfMonth** | **number** |  | [default to undefined]
**weekOfMonth** | **number** |  | [default to undefined]
**endAfterOccurrences** | **number** |  | [default to undefined]
**scheduleHistory** | [**Array&lt;ScheduleHistoryNew&gt;**](ScheduleHistoryNew.md) |  | [optional] [default to undefined]
**scheduleExceptions** | [**Array&lt;ScheduleExceptionNew&gt;**](ScheduleExceptionNew.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ScheduleNew } from './api';

const instance: ScheduleNew = {
    id,
    createdAt,
    updatedAt,
    startTime,
    endTime,
    type,
    objectId,
    frequency,
    interval,
    daysOfWeek,
    dayOfMonth,
    weekOfMonth,
    endAfterOccurrences,
    scheduleHistory,
    scheduleExceptions,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
