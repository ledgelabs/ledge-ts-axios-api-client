# AdminBannerApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createBanner**](#createbanner) | **POST** /admin/banners | |
|[**deleteBanner**](#deletebanner) | **DELETE** /admin/banners/{id} | |
|[**getAllBanners**](#getallbanners) | **GET** /admin/banners/{eventId} | |
|[**updateBanner**](#updatebanner) | **PATCH** /admin/banners/{bannerId} | |
|[**uploadBannerImages**](#uploadbannerimages) | **PATCH** /admin/banners/{id}/images | |

# **createBanner**
> PickBannerOrIdOrCreatedAtOrUpdatedAtOrStartTimeOrEndTimeOrBannerLocationOrEventIdOrLogoUrlOrDesktopImageUrlOrMobileImageUrlOrAlt createBanner(createBannerArgs)


### Example

```typescript
import {
    AdminBannerApi,
    Configuration,
    CreateBannerArgs
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminBannerApi(configuration);

let createBannerArgs: CreateBannerArgs; //

const { status, data } = await apiInstance.createBanner(
    createBannerArgs
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createBannerArgs** | **CreateBannerArgs**|  | |


### Return type

**PickBannerOrIdOrCreatedAtOrUpdatedAtOrStartTimeOrEndTimeOrBannerLocationOrEventIdOrLogoUrlOrDesktopImageUrlOrMobileImageUrlOrAlt**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Banner created |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteBanner**
> DeleteAnnouncement200Response deleteBanner()


### Example

```typescript
import {
    AdminBannerApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminBannerApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteBanner(
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
|**200** | Banner deleted |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAllBanners**
> Array<PickBannerOrIdOrCreatedAtOrUpdatedAtOrStartTimeOrEndTimeOrBannerLocationOrEventIdOrLogoUrlOrDesktopImageUrlOrMobileImageUrlOrAlt> getAllBanners()


### Example

```typescript
import {
    AdminBannerApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminBannerApi(configuration);

let eventId: string; // (default to undefined)

const { status, data } = await apiInstance.getAllBanners(
    eventId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **eventId** | [**string**] |  | defaults to undefined|


### Return type

**Array<PickBannerOrIdOrCreatedAtOrUpdatedAtOrStartTimeOrEndTimeOrBannerLocationOrEventIdOrLogoUrlOrDesktopImageUrlOrMobileImageUrlOrAlt>**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Banners fetched |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateBanner**
> PickBannerOrIdOrCreatedAtOrUpdatedAtOrStartTimeOrEndTimeOrBannerLocationOrEventIdOrLogoUrlOrDesktopImageUrlOrMobileImageUrlOrAlt updateBanner(body)


### Example

```typescript
import {
    AdminBannerApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminBannerApi(configuration);

let bannerId: string; // (default to undefined)
let body: PartialCreateBannerArgs; //

const { status, data } = await apiInstance.updateBanner(
    bannerId,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PartialCreateBannerArgs**|  | |
| **bannerId** | [**string**] |  | defaults to undefined|


### Return type

**PickBannerOrIdOrCreatedAtOrUpdatedAtOrStartTimeOrEndTimeOrBannerLocationOrEventIdOrLogoUrlOrDesktopImageUrlOrMobileImageUrlOrAlt**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Banner updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **uploadBannerImages**
> string uploadBannerImages()

This endpoint is for the old system Uploads an image to S3 and updates the event\'s image URL in the database.

### Example

```typescript
import {
    AdminBannerApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminBannerApi(configuration);

let id: string; //banner id (default to undefined)
let imageType: string; //corresponds to the DB column name (default to undefined)
let file: File; //image to upload to S3 (default to undefined)
let replaceUrl: string; //optional url to replace (optional) (default to undefined)

const { status, data } = await apiInstance.uploadBannerImages(
    id,
    imageType,
    file,
    replaceUrl
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | banner id | defaults to undefined|
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

