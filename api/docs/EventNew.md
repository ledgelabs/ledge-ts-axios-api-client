# EventNew


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**title** | **string** |  | [default to undefined]
**startTime** | **string** |  | [default to undefined]
**endTime** | **string** |  | [default to undefined]
**thumbnailUrl** | **string** |  | [default to undefined]
**maxPlayers** | **number** |  | [default to undefined]
**minPlayers** | **number** |  | [default to undefined]
**entryFee** | **number** |  | [default to undefined]
**status** | [**EventStatus**](EventStatus.md) |  | [default to undefined]
**mapCode** | **string** |  | [default to undefined]
**eventAuthorId** | **string** |  | [default to undefined]
**eventAuthor** | [**User**](User.md) |  | [optional] [default to undefined]
**gameId** | **string** |  | [default to undefined]
**game** | [**Game**](Game.md) |  | [optional] [default to undefined]
**eventChangeHistory** | [**Array&lt;EventChangeHistoryNew&gt;**](EventChangeHistoryNew.md) |  | [optional] [default to undefined]
**leaderboardNew** | [**Array&lt;LeaderboardNew&gt;**](LeaderboardNew.md) |  | [optional] [default to undefined]
**participants** | [**Array&lt;ParticipantNew&gt;**](ParticipantNew.md) |  | [optional] [default to undefined]
**raffleNew** | [**Array&lt;RaffleNew&gt;**](RaffleNew.md) |  | [optional] [default to undefined]
**questSet** | [**Array&lt;QuestSet&gt;**](QuestSet.md) |  | [optional] [default to undefined]
**hostCut** | **number** |  | [default to undefined]

## Example

```typescript
import { EventNew } from './api';

const instance: EventNew = {
    id,
    createdAt,
    updatedAt,
    title,
    startTime,
    endTime,
    thumbnailUrl,
    maxPlayers,
    minPlayers,
    entryFee,
    status,
    mapCode,
    eventAuthorId,
    eventAuthor,
    gameId,
    game,
    eventChangeHistory,
    leaderboardNew,
    participants,
    raffleNew,
    questSet,
    hostCut,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
