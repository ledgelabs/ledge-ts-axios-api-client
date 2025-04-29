# AdminUserRoleApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createUserRole**](#createuserrole) | **POST** /admin/user-roles/{email} | |
|[**deleteUserRole**](#deleteuserrole) | **DELETE** /admin/user-roles/{id} | |
|[**getUserRoles**](#getuserroles) | **GET** /admin/user-roles | |
|[**updateUserRole**](#updateuserrole) | **PATCH** /admin/user-roles/{id} | |

# **createUserRole**
> GetUserRole createUserRole(body)

Create a new user role for a given user id. User\'s can have multiple roles.

### Example

```typescript
import {
    AdminUserRoleApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminUserRoleApi(configuration);

let email: string; // (default to undefined)
let body: PickPrismaUserRoleNewUncheckedCreateInputRole; //- includes the role type to create

const { status, data } = await apiInstance.createUserRole(
    email,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PickPrismaUserRoleNewUncheckedCreateInputRole**| - includes the role type to create | |
| **email** | [**string**] |  | defaults to undefined|


### Return type

**GetUserRole**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | User role created |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteUserRole**
> DeleteAnnouncement200Response deleteUserRole()


### Example

```typescript
import {
    AdminUserRoleApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminUserRoleApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteUserRole(
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
|**200** | User role deleted |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getUserRoles**
> Array<GetUserRole> getUserRoles()


### Example

```typescript
import {
    AdminUserRoleApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminUserRoleApi(configuration);

let roles: Array<UserRoleType>; // (optional) (default to undefined)

const { status, data } = await apiInstance.getUserRoles(
    roles
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **roles** | **Array&lt;UserRoleType&gt;** |  | (optional) defaults to undefined|


### Return type

**Array<GetUserRole>**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | User roles fetched |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateUserRole**
> GetUserRole updateUserRole(body)

Update a user\'s role type

### Example

```typescript
import {
    AdminUserRoleApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminUserRoleApi(configuration);

let id: string; //- id of the user role to update (default to undefined)
let body: PickPrismaUserRoleNewUncheckedCreateInputRole; //- includes the role type to update to

const { status, data } = await apiInstance.updateUserRole(
    id,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PickPrismaUserRoleNewUncheckedCreateInputRole**| - includes the role type to update to | |
| **id** | [**string**] | - id of the user role to update | defaults to undefined|


### Return type

**GetUserRole**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | User role updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

