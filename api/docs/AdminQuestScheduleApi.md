# AdminQuestScheduleApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createQuestSchedule**](#createquestschedule) | **POST** /admin/quest-schedules | |
|[**deleteQuestSchedule**](#deletequestschedule) | **DELETE** /admin/quest-schedules/{id} | |
|[**getQuestSchedules**](#getquestschedules) | **GET** /admin/quest-schedules/{questId} | |
|[**updateQuestSchedule**](#updatequestschedule) | **PATCH** /admin/quest-schedules/{id} | |

# **createQuestSchedule**
> GetQuestScheduleResponse createQuestSchedule(createQuestScheduleArgs)


### Example

```typescript
import {
    AdminQuestScheduleApi,
    Configuration,
    CreateQuestScheduleArgs
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminQuestScheduleApi(configuration);

let createQuestScheduleArgs: CreateQuestScheduleArgs; //

const { status, data } = await apiInstance.createQuestSchedule(
    createQuestScheduleArgs
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createQuestScheduleArgs** | **CreateQuestScheduleArgs**|  | |


### Return type

**GetQuestScheduleResponse**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Quest schedule created |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteQuestSchedule**
> DeleteAnnouncement200Response deleteQuestSchedule()


### Example

```typescript
import {
    AdminQuestScheduleApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminQuestScheduleApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteQuestSchedule(
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
|**200** | Quest schedule deleted |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getQuestSchedules**
> Array<GetQuestScheduleResponse> getQuestSchedules()


### Example

```typescript
import {
    AdminQuestScheduleApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminQuestScheduleApi(configuration);

let questId: string; // (default to undefined)

const { status, data } = await apiInstance.getQuestSchedules(
    questId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **questId** | [**string**] |  | defaults to undefined|


### Return type

**Array<GetQuestScheduleResponse>**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Quest schedules fetched |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateQuestSchedule**
> GetQuestScheduleResponse updateQuestSchedule(body)


### Example

```typescript
import {
    AdminQuestScheduleApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminQuestScheduleApi(configuration);

let id: string; // (default to undefined)
let body: PartialCreateQuestScheduleArgs; //

const { status, data } = await apiInstance.updateQuestSchedule(
    id,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PartialCreateQuestScheduleArgs**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**GetQuestScheduleResponse**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Quest schedule updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

