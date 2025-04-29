# GameCodeApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**processGameCode**](#processgamecode) | **POST** /gameCode | |
|[**validateLinkingCode**](#validatelinkingcode) | **GET** /gameCode/validate-linking-code | |

# **processGameCode**
> DeleteAnnouncement200Response processGameCode(processGameCodeRequest)


### Example

```typescript
import {
    GameCodeApi,
    Configuration,
    ProcessGameCodeRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new GameCodeApi(configuration);

let processGameCodeRequest: ProcessGameCodeRequest; //

const { status, data } = await apiInstance.processGameCode(
    processGameCodeRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **processGameCodeRequest** | **ProcessGameCodeRequest**|  | |


### Return type

**DeleteAnnouncement200Response**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success: Game code processed |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validateLinkingCode**
> ValidateLinkingCode200Response validateLinkingCode()


### Example

```typescript
import {
    GameCodeApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new GameCodeApi(configuration);

let linkingCode: string; // (default to undefined)

const { status, data } = await apiInstance.validateLinkingCode(
    linkingCode
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **linkingCode** | [**string**] |  | defaults to undefined|


### Return type

**ValidateLinkingCode200Response**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Ok |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

