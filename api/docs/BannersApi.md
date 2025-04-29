# BannersApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getBanners**](#getbanners) | **GET** /banners | |

# **getBanners**
> Array<Banner> getBanners()


### Example

```typescript
import {
    BannersApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new BannersApi(configuration);

let bannerLocation: BannerLocation; // (default to undefined)
let eventId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getBanners(
    bannerLocation,
    eventId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bannerLocation** | **BannerLocation** |  | defaults to undefined|
| **eventId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<Banner>**

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

