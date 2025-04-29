# EventsNewApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**listUserEvents**](#listuserevents) | **GET** /events-new | |
|[**saveEvent**](#saveevent) | **PUT** /events-new/save | |
|[**uploadThumbnail**](#uploadthumbnail) | **PATCH** /events-new/{eventId}/thumbnail | |

# **listUserEvents**
> Array<EventNew> listUserEvents()


### Example

```typescript
import {
    EventsNewApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new EventsNewApi(configuration);

let statuses: Array<EventStatus>; // (optional) (default to undefined)

const { status, data } = await apiInstance.listUserEvents(
    statuses
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **statuses** | **Array&lt;EventStatus&gt;** |  | (optional) defaults to undefined|


### Return type

**Array<EventNew>**

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

# **saveEvent**
> EventNew saveEvent(saveEventDetailsArgs)

Requires `creator` role.

### Example

```typescript
import {
    EventsNewApi,
    Configuration,
    SaveEventDetailsArgs
} from './api';

const configuration = new Configuration();
const apiInstance = new EventsNewApi(configuration);

let saveEventDetailsArgs: SaveEventDetailsArgs; //

const { status, data } = await apiInstance.saveEvent(
    saveEventDetailsArgs
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **saveEventDetailsArgs** | **SaveEventDetailsArgs**|  | |


### Return type

**EventNew**

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

# **uploadThumbnail**
> string uploadThumbnail()

Uploads an image to S3 and updates the event\'s thumbnail URL in the database.

### Example

```typescript
import {
    EventsNewApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new EventsNewApi(configuration);

let eventId: string; //event id (default to undefined)
let file: File; //image to upload to S3 (default to undefined)
let replaceUrl: string; //optional url to replace (optional) (default to undefined)

const { status, data } = await apiInstance.uploadThumbnail(
    eventId,
    file,
    replaceUrl
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**string**] | event id | defaults to undefined|
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

