# Transaction


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**transactionType** | [**TransactionType**](TransactionType.md) |  | [default to undefined]
**userId** | **string** |  | [default to undefined]
**buyProductId** | **string** |  | [default to undefined]
**buyProductQuantity** | **number** |  | [default to undefined]
**sellProductId** | **string** |  | [default to undefined]
**sellProductQuantity** | **number** |  | [default to undefined]
**objectId** | **string** |  | [default to undefined]
**status** | [**StatusType**](StatusType.md) |  | [default to undefined]
**user** | [**User**](User.md) |  | [optional] [default to undefined]
**sellProduct** | [**Product**](Product.md) |  | [optional] [default to undefined]
**buyProduct** | [**Product**](Product.md) |  | [optional] [default to undefined]

## Example

```typescript
import { Transaction } from './api';

const instance: Transaction = {
    id,
    createdAt,
    updatedAt,
    transactionType,
    userId,
    buyProductId,
    buyProductQuantity,
    sellProductId,
    sellProductQuantity,
    objectId,
    status,
    user,
    sellProduct,
    buyProduct,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
