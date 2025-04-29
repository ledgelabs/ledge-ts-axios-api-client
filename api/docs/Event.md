# Event


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**startTime** | **string** |  | [default to undefined]
**endTime** | **string** |  | [default to undefined]
**status** | [**EventStatus**](EventStatus.md) |  | [default to undefined]
**title** | **string** |  | [default to undefined]
**subtitle** | **string** |  | [default to undefined]
**description** | **string** |  | [default to undefined]
**imageUrl** | **string** |  | [default to undefined]
**mapCode** | **string** |  | [default to undefined]
**youtubeId** | **string** |  | [default to undefined]
**videoUrl** | **string** |  | [default to undefined]
**gameId** | **string** |  | [default to undefined]
**game** | [**Game**](Game.md) |  | [optional] [default to undefined]
**draws** | [**Array&lt;Draw&gt;**](Draw.md) |  | [optional] [default to undefined]
**leaderboards** | [**Array&lt;Leaderboard&gt;**](Leaderboard.md) |  | [optional] [default to undefined]
**gameCodes** | [**Array&lt;GameCode&gt;**](GameCode.md) |  | [optional] [default to undefined]
**participants** | [**Array&lt;Participant&gt;**](Participant.md) |  | [optional] [default to undefined]
**quest** | [**Array&lt;Quest&gt;**](Quest.md) |  | [optional] [default to undefined]
**banners** | [**Array&lt;Banner&gt;**](Banner.md) |  | [optional] [default to undefined]

## Example

```typescript
import { Event } from './api';

const instance: Event = {
    id,
    createdAt,
    updatedAt,
    startTime,
    endTime,
    status,
    title,
    subtitle,
    description,
    imageUrl,
    mapCode,
    youtubeId,
    videoUrl,
    gameId,
    game,
    draws,
    leaderboards,
    gameCodes,
    participants,
    quest,
    banners,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
