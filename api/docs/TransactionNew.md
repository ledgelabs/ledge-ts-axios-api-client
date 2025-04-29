# TransactionNew


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**transactionType** | [**TransactionType**](TransactionType.md) |  | [default to undefined]
**buyerUserId** | **string** |  | [default to undefined]
**boughtProductId** | **string** |  | [default to undefined]
**boughtProductQuantity** | **number** |  | [default to undefined]
**sellerUserId** | **string** |  | [default to undefined]
**soldProductId** | **string** |  | [default to undefined]
**soldProductQuantity** | **number** |  | [default to undefined]
**objectId** | **string** |  | [default to undefined]
**status** | [**StatusType**](StatusType.md) |  | [default to undefined]
**buyer** | [**User**](User.md) |  | [optional] [default to undefined]
**seller** | [**User**](User.md) |  | [optional] [default to undefined]
**soldProduct** | [**Product**](Product.md) |  | [optional] [default to undefined]
**boughtProduct** | [**Product**](Product.md) |  | [optional] [default to undefined]

## Example

```typescript
import { TransactionNew } from './api';

const instance: TransactionNew = {
    id,
    createdAt,
    updatedAt,
    transactionType,
    buyerUserId,
    boughtProductId,
    boughtProductQuantity,
    sellerUserId,
    soldProductId,
    soldProductQuantity,
    objectId,
    status,
    buyer,
    seller,
    soldProduct,
    boughtProduct,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
