# GetEventDetailedResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**socialQuests** | [**Array&lt;GetQuestResponse&gt;**](GetQuestResponse.md) |  | [default to undefined]
**gameQuests** | [**Array&lt;GetQuestResponse&gt;**](GetQuestResponse.md) |  | [default to undefined]
**leaderboard** | [**GetEventDetailedResponseLeaderboard**](GetEventDetailedResponseLeaderboard.md) |  | [default to undefined]
**raffle** | [**Array&lt;GetEventDetailedResponseRaffleInner&gt;**](GetEventDetailedResponseRaffleInner.md) |  | [default to undefined]
**banners** | [**Array&lt;PickBannerOrIdOrCreatedAtOrUpdatedAtOrStartTimeOrEndTimeOrBannerLocationOrEventIdOrLogoUrlOrDesktopImageUrlOrMobileImageUrlOrAlt&gt;**](PickBannerOrIdOrCreatedAtOrUpdatedAtOrStartTimeOrEndTimeOrBannerLocationOrEventIdOrLogoUrlOrDesktopImageUrlOrMobileImageUrlOrAlt.md) |  | [default to undefined]
**event** | [**PickEventOrIdOrStartTimeOrEndTimeOrStatusOrTitleOrSubtitleOrDescriptionOrImageUrlOrMapCodeOrYoutubeIdOrVideoUrlOrGameId**](PickEventOrIdOrStartTimeOrEndTimeOrStatusOrTitleOrSubtitleOrDescriptionOrImageUrlOrMapCodeOrYoutubeIdOrVideoUrlOrGameId.md) |  | [default to undefined]

## Example

```typescript
import { GetEventDetailedResponse } from './api';

const instance: GetEventDetailedResponse = {
    socialQuests,
    gameQuests,
    leaderboard,
    raffle,
    banners,
    event,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
