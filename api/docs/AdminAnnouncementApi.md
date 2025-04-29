# AdminAnnouncementApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAnnouncement**](#createannouncement) | **POST** /admin/announcements | |
|[**deleteAnnouncement**](#deleteannouncement) | **DELETE** /admin/announcements/{id} | |
|[**getAllAnnouncements**](#getallannouncements) | **GET** /admin/announcements | |
|[**updateAnnouncement**](#updateannouncement) | **PATCH** /admin/announcements/{announcementId} | |

# **createAnnouncement**
> Announcement createAnnouncement(body)


### Example

```typescript
import {
    AdminAnnouncementApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminAnnouncementApi(configuration);

let body: PickPrismaAnnouncementUncheckedCreateInputMessageOrStatus; //

const { status, data } = await apiInstance.createAnnouncement(
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PickPrismaAnnouncementUncheckedCreateInputMessageOrStatus**|  | |


### Return type

**Announcement**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Announcement created |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteAnnouncement**
> DeleteAnnouncement200Response deleteAnnouncement()


### Example

```typescript
import {
    AdminAnnouncementApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminAnnouncementApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteAnnouncement(
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
|**200** | Announcement deleted |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAllAnnouncements**
> Array<Announcement> getAllAnnouncements()


### Example

```typescript
import {
    AdminAnnouncementApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminAnnouncementApi(configuration);

const { status, data } = await apiInstance.getAllAnnouncements();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<Announcement>**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Announcements fetched |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateAnnouncement**
> Announcement updateAnnouncement(body)


### Example

```typescript
import {
    AdminAnnouncementApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminAnnouncementApi(configuration);

let announcementId: string; // (default to undefined)
let body: PartialCreateAnnouncementArgs; //

const { status, data } = await apiInstance.updateAnnouncement(
    announcementId,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PartialCreateAnnouncementArgs**|  | |
| **announcementId** | [**string**] |  | defaults to undefined|


### Return type

**Announcement**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Announcement updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

