# RaffleNew


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**title** | **string** |  | [default to undefined]
**expiredTicketId** | **string** |  | [default to undefined]
**rewardDistributionMethod** | [**PrizeType**](PrizeType.md) |  | [default to undefined]
**ticketId** | **string** |  | [default to undefined]
**ticket** | [**Product**](Product.md) |  | [optional] [default to undefined]
**eventId** | **string** |  | [default to undefined]
**event** | [**EventNew**](EventNew.md) |  | [optional] [default to undefined]

## Example

```typescript
import { RaffleNew } from './api';

const instance: RaffleNew = {
    id,
    createdAt,
    updatedAt,
    title,
    expiredTicketId,
    rewardDistributionMethod,
    ticketId,
    ticket,
    eventId,
    event,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
