# AdminQuestApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**adminGetQuests**](#admingetquests) | **GET** /admin/quests/{eventId} | |
|[**createQuest**](#createquest) | **POST** /admin/quests/{gameId}/{eventId} | |
|[**deleteQuest**](#deletequest) | **DELETE** /admin/quests/{questId}/{goalId} | |
|[**updateQuest**](#updatequest) | **PATCH** /admin/quests/{questId}/{goalId} | |
|[**uploadQuestGoalImages**](#uploadquestgoalimages) | **PATCH** /admin/quests/goal/{id}/images | |

# **adminGetQuests**
> Array<GetQuestResponse> adminGetQuests()


### Example

```typescript
import {
    AdminQuestApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminQuestApi(configuration);

let eventId: string; // (default to undefined)
let questTypes: Array<QuestType>; // (default to undefined)

const { status, data } = await apiInstance.adminGetQuests(
    eventId,
    questTypes
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**string**] |  | defaults to undefined|
| **questTypes** | **Array&lt;QuestType&gt;** |  | defaults to undefined|


### Return type

**Array<GetQuestResponse>**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Quests fetched |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createQuest**
> CreateQuestResponse createQuest(createQuestGoalArgs)


### Example

```typescript
import {
    AdminQuestApi,
    Configuration,
    CreateQuestGoalArgs
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminQuestApi(configuration);

let gameId: string; // (default to undefined)
let eventId: string; // (default to undefined)
let createQuestGoalArgs: CreateQuestGoalArgs; //
let questId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.createQuest(
    gameId,
    eventId,
    createQuestGoalArgs,
    questId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createQuestGoalArgs** | **CreateQuestGoalArgs**|  | |
| **gameId** | [**string**] |  | defaults to undefined|
| **eventId** | [**string**] |  | defaults to undefined|
| **questId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**CreateQuestResponse**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Quest created |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteQuest**
> DeleteAnnouncement200Response deleteQuest()

Deletes the underlying goal and quest.

### Example

```typescript
import {
    AdminQuestApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminQuestApi(configuration);

let questId: string; // (default to undefined)
let goalId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteQuest(
    questId,
    goalId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **questId** | [**string**] |  | defaults to undefined|
| **goalId** | [**string**] |  | defaults to undefined|


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
|**200** | Quest deleted |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateQuest**
> CreateQuestResponse updateQuest(body)


### Example

```typescript
import {
    AdminQuestApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminQuestApi(configuration);

let questId: string; // (default to undefined)
let goalId: string; // (default to undefined)
let body: PartialCreateQuestGoalArgs; //

const { status, data } = await apiInstance.updateQuest(
    questId,
    goalId,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PartialCreateQuestGoalArgs**|  | |
| **questId** | [**string**] |  | defaults to undefined|
| **goalId** | [**string**] |  | defaults to undefined|


### Return type

**CreateQuestResponse**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Quest updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **uploadQuestGoalImages**
> string uploadQuestGoalImages()

Uploads an image to S3 and updates the goal\'s (Quest) image URL in the database.

### Example

```typescript
import {
    AdminQuestApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminQuestApi(configuration);

let id: string; //goal id not quest id (default to undefined)
let imageType: string; //corresponds to the DB column name (default to undefined)
let file: File; //image to upload to S3 (default to undefined)
let replaceUrl: string; //optional url to replace (optional) (default to undefined)

const { status, data } = await apiInstance.uploadQuestGoalImages(
    id,
    imageType,
    file,
    replaceUrl
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | goal id not quest id | defaults to undefined|
| **imageType** | [**string**] | corresponds to the DB column name | defaults to undefined|
| **file** | [**File**] | image to upload to S3 | defaults to undefined|
| **replaceUrl** | [**string**] | optional url to replace | (optional) defaults to undefined|


### Return type

**string**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | uploaded image url |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

