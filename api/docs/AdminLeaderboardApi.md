# AdminLeaderboardApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createLeaderboard**](#createleaderboard) | **POST** /admin/leaderboards | |
|[**deleteLeaderboard**](#deleteleaderboard) | **DELETE** /admin/leaderboards | |
|[**getLeaderboard**](#getleaderboard) | **GET** /admin/leaderboards/{eventId} | |
|[**saveLeaderboard**](#saveleaderboard) | **PUT** /admin/leaderboards | |
|[**updateLeaderboard**](#updateleaderboard) | **PATCH** /admin/leaderboards | |

# **createLeaderboard**
> CreateLeaderboardResponse createLeaderboard(createLeaderboardArgs)


### Example

```typescript
import {
    AdminLeaderboardApi,
    Configuration,
    CreateLeaderboardArgs
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardApi(configuration);

let createLeaderboardArgs: CreateLeaderboardArgs; //

const { status, data } = await apiInstance.createLeaderboard(
    createLeaderboardArgs
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createLeaderboardArgs** | **CreateLeaderboardArgs**|  | |


### Return type

**CreateLeaderboardResponse**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Leaderboard created |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteLeaderboard**
> DeleteAnnouncement200Response deleteLeaderboard()


### Example

```typescript
import {
    AdminLeaderboardApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteLeaderboard(
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
|**200** | Leaderboard deleted |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getLeaderboard**
> GetLeaderboardResponse getLeaderboard()

Note: although its possible for an event to have multiple leaderboards, this endpoint will only return the first one found b/c currently we only do events with one leaderboard. That typically means 1 leaderboard schedule starting/ending at the same time as the event itself. Get a leaderboard by event id

### Example

```typescript
import {
    AdminLeaderboardApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardApi(configuration);

let eventId: string; //- The event id (default to undefined)

const { status, data } = await apiInstance.getLeaderboard(
    eventId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**string**] | - The event id | defaults to undefined|


### Return type

**GetLeaderboardResponse**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Leaderboard fetched |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **saveLeaderboard**
> UpdateLeaderboardResponse saveLeaderboard(saveLeaderboardArgs)


### Example

```typescript
import {
    AdminLeaderboardApi,
    Configuration,
    SaveLeaderboardArgs
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardApi(configuration);

let saveLeaderboardArgs: SaveLeaderboardArgs; //

const { status, data } = await apiInstance.saveLeaderboard(
    saveLeaderboardArgs
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **saveLeaderboardArgs** | **SaveLeaderboardArgs**|  | |


### Return type

**UpdateLeaderboardResponse**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Leaderboard saved |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateLeaderboard**
> UpdateLeaderboardResponse updateLeaderboard(body)


### Example

```typescript
import {
    AdminLeaderboardApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardApi(configuration);

let id: string; // (default to undefined)
let body: PartialCreateLeaderboardArgs; //

const { status, data } = await apiInstance.updateLeaderboard(
    id,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PartialCreateLeaderboardArgs**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**UpdateLeaderboardResponse**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Leaderboard updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

