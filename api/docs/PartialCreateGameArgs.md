# PartialCreateGameArgs

Make all properties in T optional

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **string** |  | [optional] [default to undefined]
**studioId** | **string** |  | [optional] [default to undefined]
**iconUrl** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**createAccess** | [**CreateEventGameAccess**](CreateEventGameAccess.md) |  | [optional] [default to undefined]
**createEventImageUrl** | **string** |  | [optional] [default to undefined]
**clientId** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { PartialCreateGameArgs } from './api';

const instance: PartialCreateGameArgs = {
    title,
    studioId,
    iconUrl,
    description,
    createAccess,
    createEventImageUrl,
    clientId,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
