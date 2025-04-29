# QuestsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getQuests**](#getquests) | **GET** /quests | |

# **getQuests**
> PaginatedQuestGoal getQuests()


### Example

```typescript
import {
    QuestsApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new QuestsApi(configuration);

let eventId: string; // (default to undefined)
let questType: QuestType; // (default to undefined)
let page: number; // (optional) (default to 0)
let limit: number; // (optional) (default to 10)
let activityTypes: Array<ActivityType>; // (optional) (default to undefined)
let processed: boolean; // (optional) (default to undefined)

const { status, data } = await apiInstance.getQuests(
    eventId,
    questType,
    page,
    limit,
    activityTypes,
    processed
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**string**] |  | defaults to undefined|
| **questType** | **QuestType** |  | defaults to undefined|
| **page** | [**number**] |  | (optional) defaults to 0|
| **limit** | [**number**] |  | (optional) defaults to 10|
| **activityTypes** | **Array&lt;ActivityType&gt;** |  | (optional) defaults to undefined|
| **processed** | [**boolean**] |  | (optional) defaults to undefined|


### Return type

**PaginatedQuestGoal**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Ok |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

