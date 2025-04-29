# SaveEventDetailsArgs


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**eventData** | [**CreateEventArgs**](CreateEventArgs.md) |  | [default to undefined]
**leaderboardData** | [**CreateLeaderboardArgs**](CreateLeaderboardArgs.md) |  | [optional] [default to undefined]
**leaderboardRewardData** | [**CreateLeaderboardRewardArgs**](CreateLeaderboardRewardArgs.md) |  | [optional] [default to undefined]
**raffleData** | [**CreateRaffleArgsBaseRaffleRewardsArgs**](CreateRaffleArgsBaseRaffleRewardsArgs.md) |  | [optional] [default to undefined]
**gameQuestData** | [**CreateGameQuestArgs**](CreateGameQuestArgs.md) |  | [optional] [default to undefined]
**socialQuestData** | [**CreateSocialQuestArgs**](CreateSocialQuestArgs.md) |  | [optional] [default to undefined]

## Example

```typescript
import { SaveEventDetailsArgs } from './api';

const instance: SaveEventDetailsArgs = {
    eventData,
    leaderboardData,
    leaderboardRewardData,
    raffleData,
    gameQuestData,
    socialQuestData,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
