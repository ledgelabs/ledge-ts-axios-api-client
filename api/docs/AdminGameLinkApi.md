# AdminGameLinkApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createGameLink**](#creategamelink) | **POST** /admin/game-links/{gameId} | |
|[**deleteGameLink**](#deletegamelink) | **DELETE** /admin/game-links/{id} | |
|[**getGameLinks**](#getgamelinks) | **GET** /admin/game-links/{gameId} | |
|[**updateGameLink**](#updategamelink) | **PATCH** /admin/game-links/{id} | |
|[**updateGameLinks**](#updategamelinks) | **PATCH** /admin/game-links/bulkUpdate | |

# **createGameLink**
> GameLinks createGameLink(body)


### Example

```typescript
import {
    AdminGameLinkApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminGameLinkApi(configuration);

let gameId: string; // (default to undefined)
let body: PickPrismaGameLinksUncheckedCreateInputLinkTypeOrUrlOrOrderOrStatusOrGameId; //

const { status, data } = await apiInstance.createGameLink(
    gameId,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PickPrismaGameLinksUncheckedCreateInputLinkTypeOrUrlOrOrderOrStatusOrGameId**|  | |
| **gameId** | [**string**] |  | defaults to undefined|


### Return type

**GameLinks**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Game link created |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteGameLink**
> DeleteAnnouncement200Response deleteGameLink()


### Example

```typescript
import {
    AdminGameLinkApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminGameLinkApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteGameLink(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**DeleteAnnouncement200Response**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Game link deleted |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getGameLinks**
> Array<GameLinks> getGameLinks()


### Example

```typescript
import {
    AdminGameLinkApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminGameLinkApi(configuration);

let gameId: string; // (default to undefined)

const { status, data } = await apiInstance.getGameLinks(
    gameId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **gameId** | [**string**] |  | defaults to undefined|


### Return type

**Array<GameLinks>**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Game links fetched |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateGameLink**
> GameLinks updateGameLink(body)


### Example

```typescript
import {
    AdminGameLinkApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminGameLinkApi(configuration);

let id: string; // (default to undefined)
let body: PartialCreateGameLinkArgs; //

const { status, data } = await apiInstance.updateGameLink(
    id,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PartialCreateGameLinkArgs**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**GameLinks**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Game link updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateGameLinks**
> Array<GameLinks> updateGameLinks(updateGameLinksBulkArgs)


### Example

```typescript
import {
    AdminGameLinkApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminGameLinkApi(configuration);

let updateGameLinksBulkArgs: Array<UpdateGameLinksBulkArgs>; //

const { status, data } = await apiInstance.updateGameLinks(
    updateGameLinksBulkArgs
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateGameLinksBulkArgs** | **Array<UpdateGameLinksBulkArgs>**|  | |


### Return type

**Array<GameLinks>**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Game links updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

