# GameMode


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**title** | **string** |  | [default to undefined]
**description** | **string** |  | [default to undefined]
**imageUrl** | **string** |  | [default to undefined]
**mappingId** | **string** |  | [default to undefined]
**scoreTextAlias** | **string** |  | [default to undefined]
**altScoreTextAlias** | **string** |  | [default to undefined]
**gameId** | **string** |  | [default to undefined]
**game** | [**Game**](Game.md) |  | [optional] [default to undefined]
**leaderboardFactors** | [**Array&lt;LeaderboardFactorNew&gt;**](LeaderboardFactorNew.md) |  | [optional] [default to undefined]

## Example

```typescript
import { GameMode } from './api';

const instance: GameMode = {
    id,
    createdAt,
    updatedAt,
    title,
    description,
    imageUrl,
    mappingId,
    scoreTextAlias,
    altScoreTextAlias,
    gameId,
    game,
    leaderboardFactors,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
