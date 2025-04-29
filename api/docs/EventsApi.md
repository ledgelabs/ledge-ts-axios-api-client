# EventsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**generateLeaderboardWinCodes**](#generateleaderboardwincodes) | **POST** /events/generate-lb-win-codes | |
|[**getAllEvents**](#getallevents) | **GET** /events/all | |
|[**getEvent**](#getevent) | **GET** /events | |
|[**getLatestEvent**](#getlatestevent) | **GET** /events/latest/{gameId} | |
|[**getUserJoinedStatus**](#getuserjoinedstatus) | **GET** /events/join/{eventId}/status | |
|[**joinEvent**](#joinevent) | **POST** /events/join/{eventId} | |

# **generateLeaderboardWinCodes**
> DeleteAnnouncement200Response generateLeaderboardWinCodes(generateLeaderboardWinCodesRequest)

Generates a specified number of leaderboard win codes for the given game. Requires `write:game-code` permission.

### Example

```typescript
import {
    EventsApi,
    Configuration,
    GenerateLeaderboardWinCodesRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new EventsApi(configuration);

let generateLeaderboardWinCodesRequest: GenerateLeaderboardWinCodesRequest; //numOfCodes: the number of codes to generate, eventId: the id of the event to generate codes for

const { status, data } = await apiInstance.generateLeaderboardWinCodes(
    generateLeaderboardWinCodesRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **generateLeaderboardWinCodesRequest** | **GenerateLeaderboardWinCodesRequest**| numOfCodes: the number of codes to generate, eventId: the id of the event to generate codes for | |


### Return type

**DeleteAnnouncement200Response**

### Authorization

[tsoa_auth](../README.md#tsoa_auth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Success: LB win codes generated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAllEvents**
> PaginatedGetEventWithLobbyDetailsResponse getAllEvents()

Get all events sorted and filtered by status and end time. See repository for more details. Also map event details to include lobby details.

### Example

```typescript
import {
    EventsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new EventsApi(configuration);

let includeStatuses: Array<EventStatus>; // (default to undefined)
let page: number; // (optional) (default to 0)
let limit: number; // (optional) (default to 10)

const { status, data } = await apiInstance.getAllEvents(
    includeStatuses,
    page,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **includeStatuses** | **Array&lt;EventStatus&gt;** |  | defaults to undefined|
| **page** | [**number**] |  | (optional) defaults to 0|
| **limit** | [**number**] |  | (optional) defaults to 10|


### Return type

**PaginatedGetEventWithLobbyDetailsResponse**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | data: Events in sorted order based on EventStatus, pagination details |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getEvent**
> Event getEvent()


### Example

```typescript
import {
    EventsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new EventsApi(configuration);

let eventId: string; // (default to undefined)

const { status, data } = await apiInstance.getEvent(
    eventId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**string**] |  | defaults to undefined|


### Return type

**Event**

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

# **getLatestEvent**
> Event getLatestEvent()


### Example

```typescript
import {
    EventsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new EventsApi(configuration);

let gameId: string; // (default to undefined)

const { status, data } = await apiInstance.getLatestEvent(
    gameId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **gameId** | [**string**] |  | defaults to undefined|


### Return type

**Event**

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

# **getUserJoinedStatus**
> GetUserJoinedStatus200Response getUserJoinedStatus()

Get the joined status and timestamp of a user for a specific event.

### Example

```typescript
import {
    EventsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new EventsApi(configuration);

let eventId: string; //The ID of the event (default to undefined)

const { status, data } = await apiInstance.getUserJoinedStatus(
    eventId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**string**] | The ID of the event | defaults to undefined|


### Return type

**GetUserJoinedStatus200Response**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | : boolean, timestamp: Date | null } |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **joinEvent**
> DeleteAnnouncement200Response joinEvent()

Join an event with the specified eventId, userId, and timestamp.

### Example

```typescript
import {
    EventsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new EventsApi(configuration);

let eventId: string; //The ID of the event (default to undefined)

const { status, data } = await apiInstance.joinEvent(
    eventId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**string**] | The ID of the event | defaults to undefined|


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
|**200** | Success message |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

