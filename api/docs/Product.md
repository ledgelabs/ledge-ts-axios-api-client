# Product


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**type** | [**ProductType**](ProductType.md) |  | [default to undefined]
**title** | **string** |  | [default to undefined]
**subTitle** | **string** |  | [default to undefined]
**description** | **string** |  | [default to undefined]
**initialQuantity** | **number** |  | [default to undefined]
**iconUrl** | **string** |  | [default to undefined]
**gameId** | **string** |  | [default to undefined]
**raffleNew** | [**RaffleNew**](RaffleNew.md) |  | [optional] [default to undefined]
**buyTransactions** | [**Array&lt;Transaction&gt;**](Transaction.md) |  | [optional] [default to undefined]
**sellTransactions** | [**Array&lt;Transaction&gt;**](Transaction.md) |  | [optional] [default to undefined]
**goalProducts** | [**Array&lt;GoalProduct&gt;**](GoalProduct.md) |  | [optional] [default to undefined]
**userInventory** | [**Array&lt;UserInventory&gt;**](UserInventory.md) |  | [optional] [default to undefined]
**ticketDraws** | [**Array&lt;Draw&gt;**](Draw.md) |  | [optional] [default to undefined]
**expiredTicketDraws** | [**Array&lt;Draw&gt;**](Draw.md) |  | [optional] [default to undefined]
**drawProducts** | [**Array&lt;DrawProduct&gt;**](DrawProduct.md) |  | [optional] [default to undefined]
**leaderboardRewards** | [**Array&lt;LeaderboardReward&gt;**](LeaderboardReward.md) |  | [optional] [default to undefined]
**rewards** | [**Array&lt;RewardNew&gt;**](RewardNew.md) |  | [optional] [default to undefined]
**buyTransactionsNew** | [**Array&lt;TransactionNew&gt;**](TransactionNew.md) |  | [optional] [default to undefined]
**sellTransactionsNew** | [**Array&lt;TransactionNew&gt;**](TransactionNew.md) |  | [optional] [default to undefined]

## Example

```typescript
import { Product } from './api';

const instance: Product = {
    id,
    createdAt,
    updatedAt,
    type,
    title,
    subTitle,
    description,
    initialQuantity,
    iconUrl,
    gameId,
    raffleNew,
    buyTransactions,
    sellTransactions,
    goalProducts,
    userInventory,
    ticketDraws,
    expiredTicketDraws,
    drawProducts,
    leaderboardRewards,
    rewards,
    buyTransactionsNew,
    sellTransactionsNew,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
