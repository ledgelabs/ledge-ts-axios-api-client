# LeaderboardResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**status** | [**UserDrawStatus**](UserDrawStatus.md) |  | [default to undefined]
**userId** | **string** |  | [default to undefined]
**user** | [**User**](User.md) |  | [optional] [default to undefined]
**leaderboardScheduleId** | **string** |  | [default to undefined]
**leaderboardSchedule** | [**LeaderboardSchedule**](LeaderboardSchedule.md) |  | [optional] [default to undefined]
**leaderboardRewards** | [**Array&lt;LeaderboardReward&gt;**](LeaderboardReward.md) |  | [optional] [default to undefined]

## Example

```typescript
import { LeaderboardResult } from './api';

const instance: LeaderboardResult = {
    id,
    createdAt,
    updatedAt,
    status,
    userId,
    user,
    leaderboardScheduleId,
    leaderboardSchedule,
    leaderboardRewards,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
