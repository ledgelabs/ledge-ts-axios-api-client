# NotificationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**claimPrize**](#claimprize) | **PATCH** /notification/claim | |
|[**claimPrizeNew**](#claimprizenew) | **PATCH** /notification/claim-new | |
|[**createPrizeDeliveredNotification**](#createprizedeliverednotification) | **POST** /notification/prize-delivered-notifications | |
|[**deleteById**](#deletebyid) | **DELETE** /notification | |
|[**getNotifications**](#getnotifications) | **GET** /notification | |
|[**updateNotifications**](#updatenotifications) | **PATCH** /notification/notifications | |

# **claimPrize**
> CreatePrizeDeliveredNotification200Response claimPrize(claimPrizeRequest)


### Example

```typescript
import {
    NotificationApi,
    Configuration,
    ClaimPrizeRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new NotificationApi(configuration);

let claimPrizeRequest: ClaimPrizeRequest; //

const { status, data } = await apiInstance.claimPrize(
    claimPrizeRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **claimPrizeRequest** | **ClaimPrizeRequest**|  | |


### Return type

**CreatePrizeDeliveredNotification200Response**

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

# **claimPrizeNew**
> ClaimPrizeResponse claimPrizeNew(claimPrizeRequest)


### Example

```typescript
import {
    NotificationApi,
    Configuration,
    ClaimPrizeRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new NotificationApi(configuration);

let claimPrizeRequest: ClaimPrizeRequest; //

const { status, data } = await apiInstance.claimPrizeNew(
    claimPrizeRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **claimPrizeRequest** | **ClaimPrizeRequest**|  | |


### Return type

**ClaimPrizeResponse**

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

# **createPrizeDeliveredNotification**
> CreatePrizeDeliveredNotification200Response createPrizeDeliveredNotification(createPrizeDeliveredNotificationRequest)


### Example

```typescript
import {
    NotificationApi,
    Configuration,
    CreatePrizeDeliveredNotificationRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new NotificationApi(configuration);

let createPrizeDeliveredNotificationRequest: CreatePrizeDeliveredNotificationRequest; //

const { status, data } = await apiInstance.createPrizeDeliveredNotification(
    createPrizeDeliveredNotificationRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createPrizeDeliveredNotificationRequest** | **CreatePrizeDeliveredNotificationRequest**|  | |


### Return type

**CreatePrizeDeliveredNotification200Response**

### Authorization

[tsoa_auth](../README.md#tsoa_auth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Ok |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteById**
> deleteById()


### Example

```typescript
import {
    NotificationApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new NotificationApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteById(
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
|**204** | No content |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getNotifications**
> PaginatedNotificationDetailed getNotifications()


### Example

```typescript
import {
    NotificationApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new NotificationApi(configuration);

let page: number; // (optional) (default to 0)
let limit: number; // (optional) (default to 10)
let orderByCreated: 'asc' | 'desc'; // (optional) (default to undefined)

const { status, data } = await apiInstance.getNotifications(
    page,
    limit,
    orderByCreated
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **page** | [**number**] |  | (optional) defaults to 0|
| **limit** | [**number**] |  | (optional) defaults to 10|
| **orderByCreated** | [**&#39;asc&#39; | &#39;desc&#39;**]**Array<&#39;asc&#39; &#124; &#39;desc&#39;>** |  | (optional) defaults to undefined|


### Return type

**PaginatedNotificationDetailed**

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

# **updateNotifications**
> updateNotifications(updateNotificationsRequest)


### Example

```typescript
import {
    NotificationApi,
    Configuration,
    UpdateNotificationsRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new NotificationApi(configuration);

let updateNotificationsRequest: UpdateNotificationsRequest; //

const { status, data } = await apiInstance.updateNotifications(
    updateNotificationsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateNotificationsRequest** | **UpdateNotificationsRequest**|  | |


### Return type

void (empty response body)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | No content |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

