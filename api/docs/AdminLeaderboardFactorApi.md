# AdminLeaderboardFactorApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createLeaderboardFactor**](#createleaderboardfactor) | **POST** /admin/leaderboard-factors | |
|[**deleteLeaderboardFactor**](#deleteleaderboardfactor) | **DELETE** /admin/leaderboard-factors | |
|[**getLeaderboardFactor**](#getleaderboardfactor) | **GET** /admin/leaderboard-factors/{leaderboardId} | |
|[**saveLeaderboardFactor**](#saveleaderboardfactor) | **PUT** /admin/leaderboard-factors | |
|[**updateLeaderboardFactor**](#updateleaderboardfactor) | **PATCH** /admin/leaderboard-factors | |

# **createLeaderboardFactor**
> LeaderboardFactor createLeaderboardFactor(body)


### Example

```typescript
import {
    AdminLeaderboardFactorApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardFactorApi(configuration);

let body: PickPrismaLeaderboardFactorUncheckedCreateInputObjectIdOrTypeOrLeaderboardId; //

const { status, data } = await apiInstance.createLeaderboardFactor(
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PickPrismaLeaderboardFactorUncheckedCreateInputObjectIdOrTypeOrLeaderboardId**|  | |


### Return type

**LeaderboardFactor**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Leaderboard factor created |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteLeaderboardFactor**
> DeleteAnnouncement200Response deleteLeaderboardFactor()


### Example

```typescript
import {
    AdminLeaderboardFactorApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardFactorApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteLeaderboardFactor(
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
|**200** | Leaderboard factor deleted |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getLeaderboardFactor**
> PickLeaderboardFactorIdOrCreatedAtOrUpdatedAtOrObjectIdOrType getLeaderboardFactor()


### Example

```typescript
import {
    AdminLeaderboardFactorApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardFactorApi(configuration);

let leaderboardId: string; // (default to undefined)

const { status, data } = await apiInstance.getLeaderboardFactor(
    leaderboardId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **leaderboardId** | [**string**] |  | defaults to undefined|


### Return type

**PickLeaderboardFactorIdOrCreatedAtOrUpdatedAtOrObjectIdOrType**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Leaderboard factor fetched |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **saveLeaderboardFactor**
> PickLeaderboardFactorIdOrCreatedAtOrUpdatedAtOrObjectIdOrType saveLeaderboardFactor(body)


### Example

```typescript
import {
    AdminLeaderboardFactorApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardFactorApi(configuration);

let body: PartialPickPrismaLeaderboardFactorUncheckedCreateInputIdOrObjectIdOrTypeOrLeaderboardId; //

const { status, data } = await apiInstance.saveLeaderboardFactor(
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PartialPickPrismaLeaderboardFactorUncheckedCreateInputIdOrObjectIdOrTypeOrLeaderboardId**|  | |


### Return type

**PickLeaderboardFactorIdOrCreatedAtOrUpdatedAtOrObjectIdOrType**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Leaderboard factor saved |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateLeaderboardFactor**
> PickLeaderboardFactorIdOrCreatedAtOrUpdatedAtOrObjectIdOrType updateLeaderboardFactor(body)


### Example

```typescript
import {
    AdminLeaderboardFactorApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminLeaderboardFactorApi(configuration);

let id: string; // (default to undefined)
let body: PartialCreateLeaderboardFactorArgs; //

const { status, data } = await apiInstance.updateLeaderboardFactor(
    id,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PartialCreateLeaderboardFactorArgs**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**PickLeaderboardFactorIdOrCreatedAtOrUpdatedAtOrObjectIdOrType**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Leaderboard factor updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

