# AdminGameApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createExternalApiKey**](#createexternalapikey) | **POST** /admin/games/{id}/external-api-key | |
|[**createGame**](#creategame) | **POST** /admin/games | |
|[**deleteGame**](#deletegame) | **DELETE** /admin/games/{id} | |
|[**getAllExternalApiKey**](#getallexternalapikey) | **GET** /admin/games/{id}/external-api-keys | |
|[**getAllGames**](#getallgames) | **GET** /admin/games | |
|[**getGameById**](#getgamebyid) | **GET** /admin/games/{id} | |
|[**updateExternalApiKey**](#updateexternalapikey) | **PATCH** /admin/games/{id}/external-api-key | |
|[**updateExternalApiKeyBulk**](#updateexternalapikeybulk) | **PATCH** /admin/games/external-api-key/bulk | |
|[**updateGame**](#updategame) | **PATCH** /admin/games | |
|[**uploadGameImages**](#uploadgameimages) | **PATCH** /admin/games/{id}/images | |

# **createExternalApiKey**
> GetExternalApiKeyResponse createExternalApiKey()

Stores newly created external api key for a game.

### Example

```typescript
import {
    AdminGameApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminGameApi(configuration);

let id: string; //game id (default to undefined)

const { status, data } = await apiInstance.createExternalApiKey(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | game id | defaults to undefined|


### Return type

**GetExternalApiKeyResponse**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | External api key created |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createGame**
> GetGamesResponse createGame(createGameArgs)


### Example

```typescript
import {
    AdminGameApi,
    Configuration,
    CreateGameArgs
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminGameApi(configuration);

let createGameArgs: CreateGameArgs; //

const { status, data } = await apiInstance.createGame(
    createGameArgs
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createGameArgs** | **CreateGameArgs**|  | |


### Return type

**GetGamesResponse**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Game created |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteGame**
> DeleteAnnouncement200Response deleteGame()


### Example

```typescript
import {
    AdminGameApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminGameApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteGame(
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
|**200** | Game deleted |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAllExternalApiKey**
> Array<GetExternalApiKeyResponse> getAllExternalApiKey()

Retrieves the external api keys for a game.

### Example

```typescript
import {
    AdminGameApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminGameApi(configuration);

let id: string; //game id (default to undefined)

const { status, data } = await apiInstance.getAllExternalApiKey(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | game id | defaults to undefined|


### Return type

**Array<GetExternalApiKeyResponse>**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | External api key retrieved |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAllGames**
> Array<GetGamesResponse> getAllGames()


### Example

```typescript
import {
    AdminGameApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminGameApi(configuration);

const { status, data } = await apiInstance.getAllGames();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<GetGamesResponse>**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Games fetched |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getGameById**
> GetGameResponseDetailed getGameById()


### Example

```typescript
import {
    AdminGameApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminGameApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getGameById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**GetGameResponseDetailed**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Game fetched |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateExternalApiKey**
> GetExternalApiKeyResponse updateExternalApiKey()

Updates an existing external api key for a game.

### Example

```typescript
import {
    AdminGameApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminGameApi(configuration);

let id: string; //api key id (default to undefined)

const { status, data } = await apiInstance.updateExternalApiKey(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | api key id | defaults to undefined|


### Return type

**GetExternalApiKeyResponse**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | External api key updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateExternalApiKeyBulk**
> Array<GetExternalApiKeyResponse> updateExternalApiKeyBulk(updateApiKeyArgs)

Updates an existing external api key for a game.

### Example

```typescript
import {
    AdminGameApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminGameApi(configuration);

let updateApiKeyArgs: Array<UpdateApiKeyArgs>; //

const { status, data } = await apiInstance.updateExternalApiKeyBulk(
    updateApiKeyArgs
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateApiKeyArgs** | **Array<UpdateApiKeyArgs>**|  | |


### Return type

**Array<GetExternalApiKeyResponse>**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | External api keys updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateGame**
> GetGamesResponse updateGame(body)


### Example

```typescript
import {
    AdminGameApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminGameApi(configuration);

let id: string; // (default to undefined)
let body: PartialCreateGameArgs; //

const { status, data } = await apiInstance.updateGame(
    id,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PartialCreateGameArgs**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**GetGamesResponse**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Game updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **uploadGameImages**
> string uploadGameImages()

Uploads an image to S3 and updates the game\'s image URL in the database.

### Example

```typescript
import {
    AdminGameApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminGameApi(configuration);

let id: string; //game id (default to undefined)
let imageType: string; //corresponds to the DB column name (default to undefined)
let file: File; //image to upload to S3 (default to undefined)
let replaceUrl: string; //optional url to replace (optional) (default to undefined)

const { status, data } = await apiInstance.uploadGameImages(
    id,
    imageType,
    file,
    replaceUrl
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | game id | defaults to undefined|
| **imageType** | [**string**] | corresponds to the DB column name | defaults to undefined|
| **file** | [**File**] | image to upload to S3 | defaults to undefined|
| **replaceUrl** | [**string**] | optional url to replace | (optional) defaults to undefined|


### Return type

**string**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | uploaded image url |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

