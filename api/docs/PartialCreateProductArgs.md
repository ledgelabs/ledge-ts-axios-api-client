# PartialCreateProductArgs

Make all properties in T optional

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **string** |  | [optional] [default to undefined]
**type** | [**ProductType**](ProductType.md) |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**gameId** | **string** |  | [optional] [default to undefined]
**iconUrl** | **string** |  | [optional] [default to undefined]
**subTitle** | **string** |  | [optional] [default to undefined]
**initialQuantity** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { PartialCreateProductArgs } from './api';

const instance: PartialCreateProductArgs = {
    title,
    type,
    description,
    gameId,
    iconUrl,
    subTitle,
    initialQuantity,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
