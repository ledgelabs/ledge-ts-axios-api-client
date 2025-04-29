# UserDrawDetailed


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**userId** | **string** |  | [default to undefined]
**drawScheduleId** | **string** |  | [default to undefined]
**drawProductId** | **string** |  | [default to undefined]
**transactionId** | **string** |  | [default to undefined]
**status** | [**UserDrawStatus**](UserDrawStatus.md) |  | [default to undefined]
**user** | [**User**](User.md) |  | [default to undefined]
**drawSchedule** | [**DrawSchedule**](DrawSchedule.md) |  | [optional] [default to undefined]
**drawProduct** | [**DrawProductDetailed**](DrawProductDetailed.md) |  | [default to undefined]

## Example

```typescript
import { UserDrawDetailed } from './api';

const instance: UserDrawDetailed = {
    id,
    createdAt,
    updatedAt,
    userId,
    drawScheduleId,
    drawProductId,
    transactionId,
    status,
    user,
    drawSchedule,
    drawProduct,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
