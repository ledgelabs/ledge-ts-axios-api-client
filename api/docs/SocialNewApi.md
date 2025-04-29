# SocialNewApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**completeSocialQuestNew**](#completesocialquestnew) | **POST** /social-new/complete-social-new | |
|[**getConnectedSocialsNew**](#getconnectedsocialsnew) | **GET** /social-new/connected-socials-new | |
|[**removeConnectedSocialNew**](#removeconnectedsocialnew) | **DELETE** /social-new/connected-social-new | |

# **completeSocialQuestNew**
> ProgressNew completeSocialQuestNew(completeSocialQuestRequestNew)


### Example

```typescript
import {
    SocialNewApi,
    Configuration,
    CompleteSocialQuestRequestNew
} from './api';

const configuration = new Configuration();
const apiInstance = new SocialNewApi(configuration);

let completeSocialQuestRequestNew: CompleteSocialQuestRequestNew; //

const { status, data } = await apiInstance.completeSocialQuestNew(
    completeSocialQuestRequestNew
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **completeSocialQuestRequestNew** | **CompleteSocialQuestRequestNew**|  | |


### Return type

**ProgressNew**

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

# **getConnectedSocialsNew**
> Array<UserConnection> getConnectedSocialsNew()


### Example

```typescript
import {
    SocialNewApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new SocialNewApi(configuration);

let id: string; // (optional) (default to undefined)
let connectionTypes: Array<ConnectionType>; // (optional) (default to undefined)

const { status, data } = await apiInstance.getConnectedSocialsNew(
    id,
    connectionTypes
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | (optional) defaults to undefined|
| **connectionTypes** | **Array&lt;ConnectionType&gt;** |  | (optional) defaults to undefined|


### Return type

**Array<UserConnection>**

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

# **removeConnectedSocialNew**
> removeConnectedSocialNew()


### Example

```typescript
import {
    SocialNewApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new SocialNewApi(configuration);

let connectionType: ConnectionType; // (default to undefined)
let userId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.removeConnectedSocialNew(
    connectionType,
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **connectionType** | **ConnectionType** |  | defaults to undefined|
| **userId** | [**string**] |  | (optional) defaults to undefined|


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
|**204** | No content |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

