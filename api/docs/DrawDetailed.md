# DrawDetailed


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**objectId** | **string** |  | [default to undefined]
**ticketId** | **string** |  | [default to undefined]
**expiredTicketId** | **string** |  | [default to undefined]
**title** | **string** |  | [default to undefined]
**eventId** | **string** |  | [default to undefined]
**questOrientation** | [**QuestOrientation**](QuestOrientation.md) |  | [default to undefined]
**imageUrl** | **string** |  | [default to undefined]
**imageBigUrl** | **string** |  | [default to undefined]
**markdown** | **string** |  | [default to undefined]
**excludePreviousWinners** | **boolean** |  | [default to undefined]
**ticket** | [**Product**](Product.md) |  | [optional] [default to undefined]
**expiredTicket** | [**Product**](Product.md) |  | [default to undefined]
**drawProducts** | [**Array&lt;DrawProductDetailed&gt;**](DrawProductDetailed.md) |  | [default to undefined]
**drawSchedules** | [**Array&lt;DrawSchedule&gt;**](DrawSchedule.md) |  | [optional] [default to undefined]
**event** | [**Event**](Event.md) |  | [default to undefined]

## Example

```typescript
import { DrawDetailed } from './api';

const instance: DrawDetailed = {
    id,
    createdAt,
    updatedAt,
    objectId,
    ticketId,
    expiredTicketId,
    title,
    eventId,
    questOrientation,
    imageUrl,
    imageBigUrl,
    markdown,
    excludePreviousWinners,
    ticket,
    expiredTicket,
    drawProducts,
    drawSchedules,
    event,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
