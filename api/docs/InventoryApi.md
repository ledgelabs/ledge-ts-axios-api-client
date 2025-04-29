# InventoryApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getInventory**](#getinventory) | **GET** /inventory | |
|[**getItemCount**](#getitemcount) | **GET** /inventory/item-counts | |
|[**getProductIdCount**](#getproductidcount) | **GET** /inventory/products/{productId} | |
|[**getSpinCase**](#getspincase) | **GET** /inventory/SpinCase | |
|[**updateInventory**](#updateinventory) | **PATCH** /inventory | |
|[**updateProfile**](#updateprofile) | **POST** /inventory/update-profile | |

# **getInventory**
> Array<UserInventoryDetailed> getInventory()


### Example

```typescript
import {
    InventoryApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new InventoryApi(configuration);

let productTypes: Array<ProductType>; // (default to undefined)
let isDefault: boolean; // (optional) (default to undefined)
let isSeen: boolean; // (optional) (default to undefined)
let userId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getInventory(
    productTypes,
    isDefault,
    isSeen,
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **productTypes** | **Array&lt;ProductType&gt;** |  | defaults to undefined|
| **isDefault** | [**boolean**] |  | (optional) defaults to undefined|
| **isSeen** | [**boolean**] |  | (optional) defaults to undefined|
| **userId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<UserInventoryDetailed>**

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

# **getItemCount**
> InventoryItemCount getItemCount()

This should return current user\'s raffle entires and return total entries for given productId. productId CAN come from Draw table ticketId

### Example

```typescript
import {
    InventoryApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new InventoryApi(configuration);

let productId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getItemCount(
    productId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **productId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**InventoryItemCount**

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

# **getProductIdCount**
> number getProductIdCount()


### Example

```typescript
import {
    InventoryApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new InventoryApi(configuration);

let productId: string; // (default to undefined)

const { status, data } = await apiInstance.getProductIdCount(
    productId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **productId** | [**string**] |  | defaults to undefined|


### Return type

**number**

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

# **getSpinCase**
> Array<UserSpinDetailed> getSpinCase()


### Example

```typescript
import {
    InventoryApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new InventoryApi(configuration);

let spinType: ProductType; // (default to undefined)

const { status, data } = await apiInstance.getSpinCase(
    spinType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **spinType** | **ProductType** |  | defaults to undefined|


### Return type

**Array<UserSpinDetailed>**

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

# **updateInventory**
> UserInventory updateInventory(userInventory)


### Example

```typescript
import {
    InventoryApi,
    Configuration,
    UserInventory
} from './api';

const configuration = new Configuration();
const apiInstance = new InventoryApi(configuration);

let inventoryId: string; // (default to undefined)
let userInventory: UserInventory; //

const { status, data } = await apiInstance.updateInventory(
    inventoryId,
    userInventory
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userInventory** | **UserInventory**|  | |
| **inventoryId** | [**string**] |  | defaults to undefined|


### Return type

**UserInventory**

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

# **updateProfile**
> UserInventory updateProfile(updateProfileRequest)


### Example

```typescript
import {
    InventoryApi,
    Configuration,
    UpdateProfileRequest
} from './api';

const configuration = new Configuration();
const apiInstance = new InventoryApi(configuration);

let updateProfileRequest: UpdateProfileRequest; //

const { status, data } = await apiInstance.updateProfile(
    updateProfileRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateProfileRequest** | **UpdateProfileRequest**|  | |


### Return type

**UserInventory**

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

