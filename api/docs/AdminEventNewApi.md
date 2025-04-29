# AdminEventNewApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getEventDetails**](#geteventdetails) | **GET** /admin/events-new/{eventId} | |
|[**listEvents**](#listevents) | **GET** /admin/events-new | |

# **getEventDetails**
> EventNew getEventDetails()


### Example

```typescript
import {
    AdminEventNewApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminEventNewApi(configuration);

let eventId: string; // (default to undefined)

const { status, data } = await apiInstance.getEventDetails(
    eventId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**string**] |  | defaults to undefined|


### Return type

**EventNew**

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

# **listEvents**
> Array<EventNew> listEvents()


### Example

```typescript
import {
    AdminEventNewApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminEventNewApi(configuration);

const { status, data } = await apiInstance.listEvents();
```

### Parameters
This endpoint does not have any parameters.


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

