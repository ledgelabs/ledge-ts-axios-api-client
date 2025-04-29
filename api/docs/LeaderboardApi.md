# LeaderboardApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getLeaderboardScore**](#getleaderboardscore) | **GET** /leaderboard/scores | |
|[**getMostRecentLeaderboardSchedules**](#getmostrecentleaderboardschedules) | **GET** /leaderboard/recent-schedules | |

# **getLeaderboardScore**
> LeaderboardScore getLeaderboardScore()


### Example

```typescript
import {
    LeaderboardApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new LeaderboardApi(configuration);

let leaderboardScheduleId: string; // (default to undefined)
let gameId: string; // (default to undefined)

const { status, data } = await apiInstance.getLeaderboardScore(
    leaderboardScheduleId,
    gameId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **leaderboardScheduleId** | [**string**] |  | defaults to undefined|
| **gameId** | [**string**] |  | defaults to undefined|


### Return type

**LeaderboardScore**

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

# **getMostRecentLeaderboardSchedules**
> Array<LeaderboardScheduleDetailed> getMostRecentLeaderboardSchedules()


### Example

```typescript
import {
    LeaderboardApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new LeaderboardApi(configuration);

let eventId: string; // (default to undefined)
let page: number; // (optional) (default to 0)
let limit: number; // (optional) (default to 10)

const { status, data } = await apiInstance.getMostRecentLeaderboardSchedules(
    eventId,
    page,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**string**] |  | defaults to undefined|
| **page** | [**number**] |  | (optional) defaults to 0|
| **limit** | [**number**] |  | (optional) defaults to 10|


### Return type

**Array<LeaderboardScheduleDetailed>**

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

