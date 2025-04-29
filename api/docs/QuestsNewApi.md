# QuestsNewApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getGameQuestTemplates**](#getgamequesttemplates) | **GET** /quests-new/game-quest-templates | |
|[**getQuestsNew**](#getquestsnew) | **GET** /quests-new | |
|[**getSocialQuestTemplates**](#getsocialquesttemplates) | **GET** /quests-new/social-quest-templates | |

# **getGameQuestTemplates**
> Array<GameQuestTemplate> getGameQuestTemplates()


### Example

```typescript
import {
    QuestsNewApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new QuestsNewApi(configuration);

let gameId: string; // (default to undefined)

const { status, data } = await apiInstance.getGameQuestTemplates(
    gameId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **gameId** | [**string**] |  | defaults to undefined|


### Return type

**Array<GameQuestTemplate>**

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

# **getQuestsNew**
> PaginatedAny getQuestsNew()


### Example

```typescript
import {
    QuestsNewApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new QuestsNewApi(configuration);

let eventId: string; // (default to undefined)
let page: number; // (optional) (default to 0)
let limit: number; // (optional) (default to 10)
let questTypes: Array<QuestType>; // (optional) (default to undefined)
let activityTypes: Array<ActivityType>; // (optional) (default to undefined)

const { status, data } = await apiInstance.getQuestsNew(
    eventId,
    page,
    limit,
    questTypes,
    activityTypes
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**string**] |  | defaults to undefined|
| **page** | [**number**] |  | (optional) defaults to 0|
| **limit** | [**number**] |  | (optional) defaults to 10|
| **questTypes** | **Array&lt;QuestType&gt;** |  | (optional) defaults to undefined|
| **activityTypes** | **Array&lt;ActivityType&gt;** |  | (optional) defaults to undefined|


### Return type

**PaginatedAny**

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

# **getSocialQuestTemplates**
> Array<GameQuestTemplate> getSocialQuestTemplates()


### Example

```typescript
import {
    QuestsNewApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new QuestsNewApi(configuration);

let activityTypes: Array<ActivityType>; // (default to undefined)

const { status, data } = await apiInstance.getSocialQuestTemplates(
    activityTypes
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **activityTypes** | **Array&lt;ActivityType&gt;** |  | defaults to undefined|


### Return type

**Array<GameQuestTemplate>**

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

