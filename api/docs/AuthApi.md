# AuthApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAppToken**](#createapptoken) | **POST** /auth/token/{applicationType}/{socialUserId} | |
|[**getToken**](#gettoken) | **GET** /auth/token | |

# **createAppToken**
> CreateAppToken200Response createAppToken()

Call on redis service to store access token to enable social client app (e.g discord bot) to use it in subsequent API requests.

### Example

```typescript
import {
    AuthApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

let applicationType: ConnectionType; // (default to undefined)
let socialUserId: string; // (default to undefined)

const { status, data } = await apiInstance.createAppToken(
    applicationType,
    socialUserId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **applicationType** | **ConnectionType** |  | defaults to undefined|
| **socialUserId** | [**string**] |  | defaults to undefined|


### Return type

**CreateAppToken200Response**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success: token stored |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getToken**
> GetToken200Response getToken()

Not currently in use. Use case: - Game Studio Devs can call this API from Ledge App to create their own API key and access our external API.

### Example

```typescript
import {
    AuthApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

const { status, data } = await apiInstance.getToken();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**GetToken200Response**

### Authorization

[basic](../README.md#basic)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Ok |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

