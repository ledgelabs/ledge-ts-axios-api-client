# LeaderboardSchedule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**startTime** | **string** |  | [default to undefined]
**endTime** | **string** |  | [default to undefined]
**recurring** | **boolean** |  | [default to undefined]
**scheduleProcessed** | **boolean** |  | [default to undefined]
**rewardsProcessed** | **boolean** |  | [default to undefined]
**leaderboardId** | **string** |  | [default to undefined]
**leaderboard** | [**Leaderboard**](Leaderboard.md) |  | [optional] [default to undefined]
**leaderboardRewards** | [**Array&lt;LeaderboardReward&gt;**](LeaderboardReward.md) |  | [optional] [default to undefined]
**scores** | [**Array&lt;LeaderboardScore&gt;**](LeaderboardScore.md) |  | [optional] [default to undefined]
**leaderboardResults** | [**Array&lt;LeaderboardResult&gt;**](LeaderboardResult.md) |  | [optional] [default to undefined]

## Example

```typescript
import { LeaderboardSchedule } from './api';

const instance: LeaderboardSchedule = {
    id,
    createdAt,
    updatedAt,
    startTime,
    endTime,
    recurring,
    scheduleProcessed,
    rewardsProcessed,
    leaderboardId,
    leaderboard,
    leaderboardRewards,
    scores,
    leaderboardResults,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
