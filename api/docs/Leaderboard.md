# Leaderboard


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**title** | **string** |  | [default to undefined]
**scoreTextAlias** | **string** |  | [default to undefined]
**altScoreTextAlias** | **string** |  | [default to undefined]
**eventId** | **string** |  | [default to undefined]
**event** | [**Event**](Event.md) |  | [optional] [default to undefined]
**gameId** | **string** |  | [default to undefined]
**game** | [**Game**](Game.md) |  | [optional] [default to undefined]
**leaderboardSchedules** | [**Array&lt;LeaderboardSchedule&gt;**](LeaderboardSchedule.md) |  | [optional] [default to undefined]
**leaderboardFactors** | [**Array&lt;LeaderboardFactor&gt;**](LeaderboardFactor.md) |  | [optional] [default to undefined]
**leaderboardDisplay** | [**LeaderboardDisplay**](LeaderboardDisplay.md) |  | [default to undefined]

## Example

```typescript
import { Leaderboard } from './api';

const instance: Leaderboard = {
    id,
    createdAt,
    updatedAt,
    title,
    scoreTextAlias,
    altScoreTextAlias,
    eventId,
    event,
    gameId,
    game,
    leaderboardSchedules,
    leaderboardFactors,
    leaderboardDisplay,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
