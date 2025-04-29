# UserDetailed


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**originalCreationDate** | **string** |  | [default to undefined]
**authId** | **string** |  | [default to undefined]
**email** | **string** |  | [default to undefined]
**phoneNumber** | **string** |  | [default to undefined]
**name** | **string** |  | [default to undefined]
**username** | **string** |  | [default to undefined]
**usertag** | **number** |  | [default to undefined]
**code** | **string** |  | [default to undefined]
**remainingReferrals** | **number** |  | [default to undefined]
**avatarUrl** | **string** |  | [default to undefined]
**birthYear** | **number** |  | [default to undefined]
**gender** | [**Gender**](Gender.md) |  | [default to undefined]
**hasOnboarded** | **boolean** |  | [default to undefined]
**hasAcceptedLegal** | **boolean** |  | [default to undefined]
**hasAcceptedAge** | **boolean** |  | [default to undefined]
**enableNotifications** | **boolean** |  | [default to undefined]
**referredById** | **string** |  | [default to undefined]
**referredBy** | [**User**](User.md) |  | [optional] [default to undefined]
**referredUsers** | [**Array&lt;User&gt;**](User.md) |  | [optional] [default to undefined]
**mergedWith** | **string** |  | [default to undefined]
**mergedWithUser** | [**User**](User.md) |  | [default to undefined]
**externalUsers** | [**Array&lt;User&gt;**](User.md) |  | [optional] [default to undefined]
**blacklist** | [**Blacklist**](Blacklist.md) |  | [default to undefined]
**transactions** | [**Array&lt;Transaction&gt;**](Transaction.md) |  | [optional] [default to undefined]
**userDraws** | [**Array&lt;UserDraw&gt;**](UserDraw.md) |  | [optional] [default to undefined]
**leaderboardScores** | [**Array&lt;LeaderboardScore&gt;**](LeaderboardScore.md) |  | [optional] [default to undefined]
**leaderboardResult** | [**Array&lt;LeaderboardResult&gt;**](LeaderboardResult.md) |  | [optional] [default to undefined]
**notifications** | [**Array&lt;Notification&gt;**](Notification.md) |  | [optional] [default to undefined]
**userInventory** | [**Array&lt;UserInventory&gt;**](UserInventory.md) |  | [optional] [default to undefined]
**activity** | [**Array&lt;Activity&gt;**](Activity.md) |  | [optional] [default to undefined]
**userConnections** | [**Array&lt;UserConnection&gt;**](UserConnection.md) |  | [optional] [default to undefined]
**userWallets** | [**Array&lt;UserWallet&gt;**](UserWallet.md) |  | [optional] [default to undefined]
**userInstalledGames** | [**Array&lt;UserInstalledGames&gt;**](UserInstalledGames.md) |  | [optional] [default to undefined]
**gameCode** | [**Array&lt;GameCode&gt;**](GameCode.md) |  | [optional] [default to undefined]
**blacklistHistory** | [**Array&lt;BlacklistHistory&gt;**](BlacklistHistory.md) |  | [optional] [default to undefined]
**userRoles** | [**Array&lt;UserRoleNew&gt;**](UserRoleNew.md) |  | [optional] [default to undefined]
**progressNew** | [**Array&lt;ProgressNew&gt;**](ProgressNew.md) |  | [optional] [default to undefined]
**buyTransactions** | [**Array&lt;TransactionNew&gt;**](TransactionNew.md) |  | [optional] [default to undefined]
**sellTransactions** | [**Array&lt;TransactionNew&gt;**](TransactionNew.md) |  | [optional] [default to undefined]
**joinedEvents** | [**Array&lt;Participant&gt;**](Participant.md) |  | [optional] [default to undefined]
**joinedEventsNew** | [**Array&lt;ParticipantNew&gt;**](ParticipantNew.md) |  | [optional] [default to undefined]
**eventNew** | [**Array&lt;EventNew&gt;**](EventNew.md) |  | [optional] [default to undefined]
**externalId** | **string** |  | [default to undefined]
**gameId** | **string** |  | [default to undefined]
**verified** | **boolean** |  | [default to undefined]
**lastLogin** | **string** |  | [default to undefined]

## Example

```typescript
import { UserDetailed } from './api';

const instance: UserDetailed = {
    id,
    createdAt,
    updatedAt,
    originalCreationDate,
    authId,
    email,
    phoneNumber,
    name,
    username,
    usertag,
    code,
    remainingReferrals,
    avatarUrl,
    birthYear,
    gender,
    hasOnboarded,
    hasAcceptedLegal,
    hasAcceptedAge,
    enableNotifications,
    referredById,
    referredBy,
    referredUsers,
    mergedWith,
    mergedWithUser,
    externalUsers,
    blacklist,
    transactions,
    userDraws,
    leaderboardScores,
    leaderboardResult,
    notifications,
    userInventory,
    activity,
    userConnections,
    userWallets,
    userInstalledGames,
    gameCode,
    blacklistHistory,
    userRoles,
    progressNew,
    buyTransactions,
    sellTransactions,
    joinedEvents,
    joinedEventsNew,
    eventNew,
    externalId,
    gameId,
    verified,
    lastLogin,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
