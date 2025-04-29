# DrawApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**claimReward**](#claimreward) | **PATCH** /draw/claim | |
|[**getNextActiveDrawSchedule**](#getnextactivedrawschedule) | **GET** /draw/drawSchedule/active/{eventId} | |
|[**getPreviousDrawSchedules**](#getpreviousdrawschedules) | **GET** /draw/drawSchedule/previous/{objectId} | |
|[**getRaffleResult**](#getraffleresult) | **GET** /draw/raffle-result/{gameId}/{drawScheduleId} | |
|[**getRecentProcessedDrawSchedule**](#getrecentprocesseddrawschedule) | **GET** /draw/recent-draw-schedule/{eventId} | |

# **claimReward**
> UserDraw claimReward()


### Example

```typescript
import {
    DrawApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new DrawApi(configuration);

let gameId: string; // (default to undefined)
let drawScheduleId: string; // (default to undefined)

const { status, data } = await apiInstance.claimReward(
    gameId,
    drawScheduleId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **gameId** | [**string**] |  | defaults to undefined|
| **drawScheduleId** | [**string**] |  | defaults to undefined|


### Return type

**UserDraw**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | null if this user has not won, therefore cannot claim the raffle prize. Otherwise, returns UserDraw with lastest status. |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getNextActiveDrawSchedule**
> DrawScheduleDetailed getNextActiveDrawSchedule()


### Example

```typescript
import {
    DrawApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new DrawApi(configuration);

let eventId: string; // (default to undefined)

const { status, data } = await apiInstance.getNextActiveDrawSchedule(
    eventId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**string**] |  | defaults to undefined|


### Return type

**DrawScheduleDetailed**

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

# **getPreviousDrawSchedules**
> Array<ProcessedDrawSchedule> getPreviousDrawSchedules()


### Example

```typescript
import {
    DrawApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new DrawApi(configuration);

let objectId: string; // (default to undefined)

const { status, data } = await apiInstance.getPreviousDrawSchedules(
    objectId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **objectId** | [**string**] |  | defaults to undefined|


### Return type

**Array<ProcessedDrawSchedule>**

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

# **getRaffleResult**
> UserDraw getRaffleResult()

Since a raffle result (UserDraw) claimable period expires in n days after an event ends, before fetching the raffle result, we need to check and update the UserDraw status accordingly.

### Example

```typescript
import {
    DrawApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new DrawApi(configuration);

let gameId: string; // (default to undefined)
let drawScheduleId: string; // (default to undefined)

const { status, data } = await apiInstance.getRaffleResult(
    gameId,
    drawScheduleId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **gameId** | [**string**] |  | defaults to undefined|
| **drawScheduleId** | [**string**] |  | defaults to undefined|


### Return type

**UserDraw**

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

# **getRecentProcessedDrawSchedule**
> ProcessedDrawSchedule getRecentProcessedDrawSchedule()


### Example

```typescript
import {
    DrawApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new DrawApi(configuration);

let eventId: string; // (default to undefined)

const { status, data } = await apiInstance.getRecentProcessedDrawSchedule(
    eventId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**string**] |  | defaults to undefined|


### Return type

**ProcessedDrawSchedule**

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

