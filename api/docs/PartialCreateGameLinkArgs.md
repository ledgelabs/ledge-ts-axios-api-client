# PartialCreateGameLinkArgs

Make all properties in T optional

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | [**AccessStatus**](AccessStatus.md) |  | [optional] [default to undefined]
**gameId** | **string** |  | [optional] [default to undefined]
**linkType** | [**LinkType**](LinkType.md) |  | [optional] [default to undefined]
**url** | **string** |  | [optional] [default to undefined]
**order** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { PartialCreateGameLinkArgs } from './api';

const instance: PartialCreateGameLinkArgs = {
    status,
    gameId,
    linkType,
    url,
    order,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
