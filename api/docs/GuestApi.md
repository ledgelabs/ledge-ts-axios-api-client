# GuestApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getActiveAnnouncement**](#getactiveannouncement) | **GET** /guest/active-announcement | |

# **getActiveAnnouncement**
> Announcement getActiveAnnouncement()


### Example

```typescript
import {
    GuestApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new GuestApi(configuration);

const { status, data } = await apiInstance.getActiveAnnouncement();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Announcement**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Ok |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

