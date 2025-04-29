# AdminLeaderboardRewardApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createLeaderboardRewards**](#createleaderboardrewards) | **POST** /admin/leaderboard-rewards | |
|[**deleteLeaderboardReward**](#deleteleaderboardreward) | **DELETE** /admin/leaderboard-rewards | |
|[**getLeaderboardRewards**](#getleaderboardrewards) | **GET** /admin/leaderboard-rewards/{leaderboardScheduleId} | |
|[**getLeaderboardRewardsSummary**](#getleaderboardrewardssummary) | **GET** /admin/leaderboard-rewards/summary/{leaderboardScheduleId} | |
|[**saveLeaderboardRewards**](#saveleaderboardrewards) | **PUT** /admin/leaderboard-rewards | |
|[**updateLeaderboardRewards**](#updateleaderboardrewards) | **PATCH** /admin/leaderboard-rewards | |

# **createLeaderboardRewards**
> BatchPayload createLeaderboardRewards(createLeaderboardRewardsArgs)


### Example

```typescript
import {
    AdminLeaderboardRewardApi,
    Configuration,
    CreateLeaderboardRewardsArgs
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardRewardApi(configuration);

let createLeaderboardRewardsArgs: CreateLeaderboardRewardsArgs; //

const { status, data } = await apiInstance.createLeaderboardRewards(
    createLeaderboardRewardsArgs
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createLeaderboardRewardsArgs** | **CreateLeaderboardRewardsArgs**|  | |


### Return type

**BatchPayload**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Leaderboard rewards created |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteLeaderboardReward**
> DeleteAnnouncement200Response deleteLeaderboardReward()


### Example

```typescript
import {
    AdminLeaderboardRewardApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardRewardApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteLeaderboardReward(
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
|**200** | Leaderboard reward deleted |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getLeaderboardRewards**
> Array<PickLeaderboardRewardIdOrCreatedAtOrUpdatedAtOrQuantityOrRewardPlaceOrProductIdOrProduct> getLeaderboardRewards()


### Example

```typescript
import {
    AdminLeaderboardRewardApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardRewardApi(configuration);

let leaderboardScheduleId: string; // (default to undefined)

const { status, data } = await apiInstance.getLeaderboardRewards(
    leaderboardScheduleId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **leaderboardScheduleId** | [**string**] |  | defaults to undefined|


### Return type

**Array<PickLeaderboardRewardIdOrCreatedAtOrUpdatedAtOrQuantityOrRewardPlaceOrProductIdOrProduct>**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Leaderboard rewards detailed fetched |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getLeaderboardRewardsSummary**
> Array<GetLeaderboardRewardSummaryResponse> getLeaderboardRewardsSummary()


### Example

```typescript
import {
    AdminLeaderboardRewardApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardRewardApi(configuration);

let leaderboardScheduleId: string; // (default to undefined)

const { status, data } = await apiInstance.getLeaderboardRewardsSummary(
    leaderboardScheduleId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **leaderboardScheduleId** | [**string**] |  | defaults to undefined|


### Return type

**Array<GetLeaderboardRewardSummaryResponse>**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Leaderboard rewards summary fetched |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **saveLeaderboardRewards**
> Array<PickLeaderboardRewardIdOrCreatedAtOrUpdatedAtOrQuantityOrRewardPlaceOrProductIdOrProduct> saveLeaderboardRewards(body)


### Example

```typescript
import {
    AdminLeaderboardRewardApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardRewardApi(configuration);

let body: CreateLeaderboardRewardsArgs; //

const { status, data } = await apiInstance.saveLeaderboardRewards(
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **CreateLeaderboardRewardsArgs**|  | |


### Return type

**Array<PickLeaderboardRewardIdOrCreatedAtOrUpdatedAtOrQuantityOrRewardPlaceOrProductIdOrProduct>**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Leaderboard rewards created/updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateLeaderboardRewards**
> PickLeaderboardRewardIdOrCreatedAtOrUpdatedAtOrQuantityOrRewardPlaceOrProductIdOrProduct updateLeaderboardRewards(body)


### Example

```typescript
import {
    AdminLeaderboardRewardApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardRewardApi(configuration);

let id: string; // (default to undefined)
let body: PickPrismaLeaderboardRewardUncheckedCreateInputQuantityOrRewardPlaceOrProductIdOrLeaderboardScheduleId; //

const { status, data } = await apiInstance.updateLeaderboardRewards(
    id,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PickPrismaLeaderboardRewardUncheckedCreateInputQuantityOrRewardPlaceOrProductIdOrLeaderboardScheduleId**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**PickLeaderboardRewardIdOrCreatedAtOrUpdatedAtOrQuantityOrRewardPlaceOrProductIdOrProduct**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Leaderboard reward updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

