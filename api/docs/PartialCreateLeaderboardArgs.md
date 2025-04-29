# PartialCreateLeaderboardArgs

Make all properties in T optional

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **string** |  | [optional] [default to undefined]
**scoreTextAlias** | **string** |  | [optional] [default to undefined]
**eventId** | **string** |  | [optional] [default to undefined]
**gameId** | **string** |  | [optional] [default to undefined]
**leaderboardDisplay** | [**LeaderboardDisplay**](LeaderboardDisplay.md) |  | [optional] [default to undefined]

## Example

```typescript
import { PartialCreateLeaderboardArgs } from './api';

const instance: PartialCreateLeaderboardArgs = {
    title,
    scoreTextAlias,
    eventId,
    gameId,
    leaderboardDisplay,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
