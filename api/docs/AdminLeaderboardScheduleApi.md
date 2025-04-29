# AdminLeaderboardScheduleApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createLeaderboardSchedule**](#createleaderboardschedule) | **POST** /admin/leaderboard-schedules | |
|[**deleteLeaderboardSchedule**](#deleteleaderboardschedule) | **DELETE** /admin/leaderboard-schedules/{id} | |
|[**getLeaderboardSchedules**](#getleaderboardschedules) | **GET** /admin/leaderboard-schedules/{leaderboardId} | |
|[**updateLeaderboardSchedule**](#updateleaderboardschedule) | **PATCH** /admin/leaderboard-schedules/{id} | |

# **createLeaderboardSchedule**
> PickLeaderboardScheduleOrIdOrCreatedAtOrUpdatedAtOrStartTimeOrEndTimeOrScheduleProcessedOrRewardsProcessed createLeaderboardSchedule(body)


### Example

```typescript
import {
    AdminLeaderboardScheduleApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardScheduleApi(configuration);

let body: PickPrismaLeaderboardScheduleUncheckedCreateInputStartTimeOrEndTimeOrScheduleProcessedOrRewardsProcessedOrLeaderboardId; //

const { status, data } = await apiInstance.createLeaderboardSchedule(
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PickPrismaLeaderboardScheduleUncheckedCreateInputStartTimeOrEndTimeOrScheduleProcessedOrRewardsProcessedOrLeaderboardId**|  | |


### Return type

**PickLeaderboardScheduleOrIdOrCreatedAtOrUpdatedAtOrStartTimeOrEndTimeOrScheduleProcessedOrRewardsProcessed**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Leaderboard schedule created |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteLeaderboardSchedule**
> DeleteAnnouncement200Response deleteLeaderboardSchedule()


### Example

```typescript
import {
    AdminLeaderboardScheduleApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardScheduleApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteLeaderboardSchedule(
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
|**200** | Leaderboard schedule deleted |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getLeaderboardSchedules**
> Array<PickLeaderboardScheduleOrIdOrCreatedAtOrUpdatedAtOrStartTimeOrEndTimeOrScheduleProcessedOrRewardsProcessed> getLeaderboardSchedules()


### Example

```typescript
import {
    AdminLeaderboardScheduleApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardScheduleApi(configuration);

let leaderboardId: string; // (default to undefined)

const { status, data } = await apiInstance.getLeaderboardSchedules(
    leaderboardId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **leaderboardId** | [**string**] |  | defaults to undefined|


### Return type

**Array<PickLeaderboardScheduleOrIdOrCreatedAtOrUpdatedAtOrStartTimeOrEndTimeOrScheduleProcessedOrRewardsProcessed>**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Leaderboard schedules fetched |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateLeaderboardSchedule**
> PickLeaderboardScheduleOrIdOrCreatedAtOrUpdatedAtOrStartTimeOrEndTimeOrScheduleProcessedOrRewardsProcessed updateLeaderboardSchedule(body)


### Example

```typescript
import {
    AdminLeaderboardScheduleApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardScheduleApi(configuration);

let id: string; // (default to undefined)
let body: PartialCreateLeaderboardScheduleArgs; //

const { status, data } = await apiInstance.updateLeaderboardSchedule(
    id,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PartialCreateLeaderboardScheduleArgs**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**PickLeaderboardScheduleOrIdOrCreatedAtOrUpdatedAtOrStartTimeOrEndTimeOrScheduleProcessedOrRewardsProcessed**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Leaderboard schedule updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

