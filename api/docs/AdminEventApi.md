# AdminEventApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**adminGetEvent**](#admingetevent) | **GET** /admin/events/{id} | |
|[**adminGetEvents**](#admingetevents) | **GET** /admin/events | |
|[**createEvent**](#createevent) | **POST** /admin/events | |
|[**deleteEvent**](#deleteevent) | **DELETE** /admin/events/{id} | |
|[**updateEvent**](#updateevent) | **PATCH** /admin/events/{eventId} | |
|[**uploadEventImages**](#uploadeventimages) | **PATCH** /admin/events/{id}/images | |

# **adminGetEvent**
> GetEventDetailedResponse adminGetEvent()

This endpoint is for the old system

### Example

```typescript
import {
    AdminEventApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminEventApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.adminGetEvent(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**GetEventDetailedResponse**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Event fetched |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **adminGetEvents**
> Array<PickEventOrIdOrStartTimeOrEndTimeOrStatusOrTitleOrSubtitleOrDescriptionOrImageUrlOrMapCodeOrYoutubeIdOrVideoUrlOrGameId> adminGetEvents()


### Example

```typescript
import {
    AdminEventApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminEventApi(configuration);

const { status, data } = await apiInstance.adminGetEvents();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<PickEventOrIdOrStartTimeOrEndTimeOrStatusOrTitleOrSubtitleOrDescriptionOrImageUrlOrMapCodeOrYoutubeIdOrVideoUrlOrGameId>**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Events fetched |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createEvent**
> PickEventOrIdOrStartTimeOrEndTimeOrStatusOrTitleOrSubtitleOrDescriptionOrImageUrlOrMapCodeOrYoutubeIdOrVideoUrlOrGameId createEvent(createEventArgs)

This endpoint is for the old system

### Example

```typescript
import {
    AdminEventApi,
    Configuration,
    CreateEventArgs
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminEventApi(configuration);

let createEventArgs: CreateEventArgs; //

const { status, data } = await apiInstance.createEvent(
    createEventArgs
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createEventArgs** | **CreateEventArgs**|  | |


### Return type

**PickEventOrIdOrStartTimeOrEndTimeOrStatusOrTitleOrSubtitleOrDescriptionOrImageUrlOrMapCodeOrYoutubeIdOrVideoUrlOrGameId**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Event created |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteEvent**
> DeleteAnnouncement200Response deleteEvent()

This endpoint is for the old system

### Example

```typescript
import {
    AdminEventApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminEventApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteEvent(
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
|**200** | Event deleted |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateEvent**
> PickEventOrIdOrStartTimeOrEndTimeOrStatusOrTitleOrSubtitleOrDescriptionOrImageUrlOrMapCodeOrYoutubeIdOrVideoUrlOrGameId updateEvent(body)

This endpoint is for the old system

### Example

```typescript
import {
    AdminEventApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminEventApi(configuration);

let eventId: string; // (default to undefined)
let body: PartialCreateEventArgs; //

const { status, data } = await apiInstance.updateEvent(
    eventId,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PartialCreateEventArgs**|  | |
| **eventId** | [**string**] |  | defaults to undefined|


### Return type

**PickEventOrIdOrStartTimeOrEndTimeOrStatusOrTitleOrSubtitleOrDescriptionOrImageUrlOrMapCodeOrYoutubeIdOrVideoUrlOrGameId**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Event updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **uploadEventImages**
> string uploadEventImages()

This endpoint is for the old system Uploads an image to S3 and updates the event\'s image URL in the database.

### Example

```typescript
import {
    AdminEventApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminEventApi(configuration);

let id: string; //event id (default to undefined)
let imageType: string; //corresponds to the DB column name (default to undefined)
let file: File; //image to upload to S3 (default to undefined)
let replaceUrl: string; //optional url to replace (optional) (default to undefined)

const { status, data } = await apiInstance.uploadEventImages(
    id,
    imageType,
    file,
    replaceUrl
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | event id | defaults to undefined|
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

