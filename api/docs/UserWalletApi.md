# UserWalletApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getUserWallets**](#getuserwallets) | **GET** /user-wallet | |
|[**storeSolanaUserWalletToDB**](#storesolanauserwallettodb) | **POST** /user-wallet | |
|[**updateUserWallet**](#updateuserwallet) | **PATCH** /user-wallet | |

# **getUserWallets**
> Array<UserWallet> getUserWallets()


### Example

```typescript
import {
    UserWalletApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserWalletApi(configuration);

const { status, data } = await apiInstance.getUserWallets();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<UserWallet>**

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

# **storeSolanaUserWalletToDB**
> UserWallet storeSolanaUserWalletToDB()


### Example

```typescript
import {
    UserWalletApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new UserWalletApi(configuration);

const { status, data } = await apiInstance.storeSolanaUserWalletToDB();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**UserWallet**

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

# **updateUserWallet**
> updateUserWallet(updateUserWalletRequest)


### Example

```typescript
import {
    UserWalletApi,
    Configuration,
    UpdateUserWalletRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new UserWalletApi(configuration);

let updateUserWalletRequest: UpdateUserWalletRequest; //

const { status, data } = await apiInstance.updateUserWallet(
    updateUserWalletRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateUserWalletRequest** | **UpdateUserWalletRequest**|  | |


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

