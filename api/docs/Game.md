# Game


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**studioId** | **string** |  | [default to undefined]
**title** | **string** |  | [default to undefined]
**description** | **string** |  | [default to undefined]
**iconUrl** | **string** |  | [default to undefined]
**clientId** | **string** |  | [default to undefined]
**createAccess** | [**CreateEventGameAccess**](CreateEventGameAccess.md) |  | [default to undefined]
**createEventImageUrl** | **string** |  | [default to undefined]
**apiKeys** | [**Array&lt;ApiKey&gt;**](ApiKey.md) |  | [optional] [default to undefined]
**leaderboards** | [**Array&lt;Leaderboard&gt;**](Leaderboard.md) |  | [optional] [default to undefined]
**userInstalledGames** | [**Array&lt;UserInstalledGames&gt;**](UserInstalledGames.md) |  | [optional] [default to undefined]
**quests** | [**Array&lt;Quest&gt;**](Quest.md) |  | [optional] [default to undefined]
**gameCode** | [**Array&lt;GameCode&gt;**](GameCode.md) |  | [optional] [default to undefined]
**events** | [**Array&lt;Event&gt;**](Event.md) |  | [optional] [default to undefined]
**links** | [**Array&lt;GameLinks&gt;**](GameLinks.md) |  | [optional] [default to undefined]
**eventNew** | [**Array&lt;EventNew&gt;**](EventNew.md) |  | [optional] [default to undefined]
**gameModes** | [**Array&lt;GameMode&gt;**](GameMode.md) |  | [optional] [default to undefined]
**gameQuestTemplates** | [**Array&lt;GameQuestTemplate&gt;**](GameQuestTemplate.md) |  | [optional] [default to undefined]

## Example

```typescript
import { Game } from './api';

const instance: Game = {
    id,
    createdAt,
    updatedAt,
    studioId,
    title,
    description,
    iconUrl,
    clientId,
    createAccess,
    createEventImageUrl,
    apiKeys,
    leaderboards,
    userInstalledGames,
    quests,
    gameCode,
    events,
    links,
    eventNew,
    gameModes,
    gameQuestTemplates,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
