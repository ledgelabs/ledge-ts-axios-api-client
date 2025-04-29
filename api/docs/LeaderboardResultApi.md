# LeaderboardResultApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getLeaderboardResults**](#getleaderboardresults) | **GET** /leaderboard-results | Get leaderboard results for a given event|

# **getLeaderboardResults**
> Array<any> getLeaderboardResults()


### Example

```typescript
import {
    LeaderboardResultApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new LeaderboardResultApi(configuration);

let eventId: string; //The ID of the event to get leaderboard results for. (default to undefined)

const { status, data } = await apiInstance.getLeaderboardResults(
    eventId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**string**] | The ID of the event to get leaderboard results for. | defaults to undefined|


### Return type

**Array<any>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | The leaderboard results for the given event. |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

