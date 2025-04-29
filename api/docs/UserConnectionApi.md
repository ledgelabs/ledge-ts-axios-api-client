# UserConnectionApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**connectSocial**](#connectsocial) | **POST** /user-connection | |
|[**getUserConnections**](#getuserconnections) | **GET** /user-connection | |
|[**removeConnectedSocial**](#removeconnectedsocial) | **DELETE** /user-connection | |

# **connectSocial**
> CreateUserConnectionResponse connectSocial(createUserConnectionRequest)


### Example

```typescript
import {
    UserConnectionApi,
    Configuration,
    CreateUserConnectionRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new UserConnectionApi(configuration);

let createUserConnectionRequest: CreateUserConnectionRequest; //

const { status, data } = await apiInstance.connectSocial(
    createUserConnectionRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createUserConnectionRequest** | **CreateUserConnectionRequest**|  | |


### Return type

**CreateUserConnectionResponse**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | User connection created |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUserConnections**
> Array<GetUserConnectionResponse> getUserConnections()


### Example

```typescript
import {
    UserConnectionApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserConnectionApi(configuration);

let connectionTypes: Array<ConnectionType>; // (default to undefined)

const { status, data } = await apiInstance.getUserConnections(
    connectionTypes
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **connectionTypes** | **Array&lt;ConnectionType&gt;** |  | defaults to undefined|


### Return type

**Array<GetUserConnectionResponse>**

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

# **removeConnectedSocial**
> removeConnectedSocial()


### Example

```typescript
import {
    UserConnectionApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserConnectionApi(configuration);

let connectionType: ConnectionType; // (default to undefined)
let userId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.removeConnectedSocial(
    connectionType,
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **connectionType** | **ConnectionType** |  | defaults to undefined|
| **userId** | [**string**] |  | (optional) defaults to undefined|


### Return type

void (empty response body)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | No content |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

