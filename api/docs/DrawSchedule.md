# DrawSchedule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [default to undefined]
**createdAt** | **string** |  | [default to undefined]
**updatedAt** | **string** |  | [default to undefined]
**startTime** | **string** |  | [default to undefined]
**endTime** | **string** |  | [default to undefined]
**recurring** | **boolean** |  | [default to undefined]
**drawId** | **string** |  | [default to undefined]
**processed** | **boolean** |  | [default to undefined]
**draw** | [**Draw**](Draw.md) |  | [optional] [default to undefined]
**userDraws** | [**Array&lt;UserDraw&gt;**](UserDraw.md) |  | [optional] [default to undefined]

## Example

```typescript
import { DrawSchedule } from './api';

const instance: DrawSchedule = {
    id,
    createdAt,
    updatedAt,
    startTime,
    endTime,
    recurring,
    drawId,
    processed,
    draw,
    userDraws,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
