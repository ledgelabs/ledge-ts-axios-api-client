# SocialApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**completeSocialQuest**](#completesocialquest) | **POST** /social/complete-social | |
|[**createSociaQuest**](#createsociaquest) | **POST** /social/quest | |

# **completeSocialQuest**
> CompleteSocialQuestResponse completeSocialQuest(completeSocialQuestRequest)

If there is no goalId, still save the user connection details. If there is a goalId, complete the quest/goal and reward the user. If the quest is completed, update the leaderboard score.

### Example

```typescript
import {
    SocialApi,
    Configuration,
    CompleteSocialQuestRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new SocialApi(configuration);

let completeSocialQuestRequest: CompleteSocialQuestRequest; //

const { status, data } = await apiInstance.completeSocialQuest(
    completeSocialQuestRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **completeSocialQuestRequest** | **CompleteSocialQuestRequest**|  | |


### Return type

**CompleteSocialQuestResponse**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Ok |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createSociaQuest**
> Goal createSociaQuest(socialQuestCreateInput)


### Example

```typescript
import {
    SocialApi,
    Configuration,
    SocialQuestCreateInput
} from './api';

const configuration = new Configuration();
const apiInstance = new SocialApi(configuration);

let socialQuestCreateInput: SocialQuestCreateInput; //

const { status, data } = await apiInstance.createSociaQuest(
    socialQuestCreateInput
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **socialQuestCreateInput** | **SocialQuestCreateInput**|  | |


### Return type

**Goal**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Ok |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

