# GamesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getEventGames**](#geteventgames) | **GET** /games/event | |
|[**getGame**](#getgame) | **GET** /games/{eventId} | |

# **getEventGames**
> PaginatedEventGame getEventGames()

This endpoint returns games in which Ledge users can create events for.

### Example

```typescript
import {
    GamesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new GamesApi(configuration);

let page: number; //- The current page index (default is 0). (optional) (default to 0)
let limit: number; //- The number of items per page (default is 10). (optional) (default to 10)

const { status, data } = await apiInstance.getEventGames(
    page,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **page** | [**number**] | - The current page index (default is 0). | (optional) defaults to 0|
| **limit** | [**number**] | - The number of items per page (default is 10). | (optional) defaults to 10|


### Return type

**PaginatedEventGame**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | A paginated list of games with metadata. |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getGame**
> GameDetailed getGame()


### Example

```typescript
import {
    GamesApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new GamesApi(configuration);

let eventId: string; // (default to undefined)

const { status, data } = await apiInstance.getGame(
    eventId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**string**] |  | defaults to undefined|


### Return type

**GameDetailed**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Ok |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

