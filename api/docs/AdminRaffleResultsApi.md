# AdminRaffleResultsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getRaffleWinnersByDrawScheduleId**](#getrafflewinnersbydrawscheduleid) | **GET** /admin/raffle-results/winners | Retrieve the raffle winners by draw schedule id|

# **getRaffleWinnersByDrawScheduleId**
> Array<GetRaffleResultsResponse> getRaffleWinnersByDrawScheduleId()


### Example

```typescript
import {
    AdminRaffleResultsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminRaffleResultsApi(configuration);

let drawScheduleId: string; //unique id per draw schedule (e.g \"ledge-fortnite-event-draw-schedule\") (default to undefined)

const { status, data } = await apiInstance.getRaffleWinnersByDrawScheduleId(
    drawScheduleId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **drawScheduleId** | [**string**] | unique id per draw schedule (e.g \&quot;ledge-fortnite-event-draw-schedule\&quot;) | defaults to undefined|


### Return type

**Array<GetRaffleResultsResponse>**

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

