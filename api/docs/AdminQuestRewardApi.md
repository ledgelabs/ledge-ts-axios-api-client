# AdminQuestRewardApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createManyQuestRewards**](#createmanyquestrewards) | **POST** /admin/quest-rewards/bulk | |
|[**createQuestReward**](#createquestreward) | **POST** /admin/quest-rewards | |
|[**deleteQuestReward**](#deletequestreward) | **DELETE** /admin/quest-rewards/{id} | |
|[**updateQuestReward**](#updatequestreward) | **PATCH** /admin/quest-rewards | |

# **createManyQuestRewards**
> BatchPayload createManyQuestRewards(createQuestRewardArgs)


### Example

```typescript
import {
    AdminQuestRewardApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminQuestRewardApi(configuration);

let createQuestRewardArgs: Array<CreateQuestRewardArgs>; //

const { status, data } = await apiInstance.createManyQuestRewards(
    createQuestRewardArgs
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createQuestRewardArgs** | **Array<CreateQuestRewardArgs>**|  | |


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
|**201** | Quest rewards created |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createQuestReward**
> GetQuestRewardResponse createQuestReward(createQuestRewardArgs)


### Example

```typescript
import {
    AdminQuestRewardApi,
    Configuration,
    CreateQuestRewardArgs
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminQuestRewardApi(configuration);

let createQuestRewardArgs: CreateQuestRewardArgs; //

const { status, data } = await apiInstance.createQuestReward(
    createQuestRewardArgs
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createQuestRewardArgs** | **CreateQuestRewardArgs**|  | |


### Return type

**GetQuestRewardResponse**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Quest reward created |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteQuestReward**
> deleteQuestReward()


### Example

```typescript
import {
    AdminQuestRewardApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminQuestRewardApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteQuestReward(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

void (empty response body)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | Quest reward deleted |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateQuestReward**
> GetQuestRewardResponse updateQuestReward(body)


### Example

```typescript
import {
    AdminQuestRewardApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminQuestRewardApi(configuration);

let body: PartialCreateQuestRewardArgs; //

const { status, data } = await apiInstance.updateQuestReward(
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PartialCreateQuestRewardArgs**|  | |


### Return type

**GetQuestRewardResponse**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Quest reward updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

