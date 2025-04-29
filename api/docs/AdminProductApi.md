# AdminProductApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createProduct**](#createproduct) | **POST** /admin/products | |
|[**deleteProduct**](#deleteproduct) | **DELETE** /admin/products/{id} | |
|[**getAllProducts**](#getallproducts) | **GET** /admin/products | |
|[**getProduct**](#getproduct) | **GET** /admin/products/{id} | |
|[**updateProduct**](#updateproduct) | **PATCH** /admin/products | |
|[**uploadProductImages**](#uploadproductimages) | **PATCH** /admin/products/{id}/images | |

# **createProduct**
> PickProductOrIdOrCreatedAtOrUpdatedAtOrTypeOrTitleOrSubTitleOrDescriptionOrInitialQuantityOrIconUrlOrGameId createProduct(createProductArgs)


### Example

```typescript
import {
    AdminProductApi,
    Configuration,
    CreateProductArgs
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminProductApi(configuration);

let createProductArgs: CreateProductArgs; //

const { status, data } = await apiInstance.createProduct(
    createProductArgs
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createProductArgs** | **CreateProductArgs**|  | |


### Return type

**PickProductOrIdOrCreatedAtOrUpdatedAtOrTypeOrTitleOrSubTitleOrDescriptionOrInitialQuantityOrIconUrlOrGameId**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Product created |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteProduct**
> DeleteAnnouncement200Response deleteProduct()


### Example

```typescript
import {
    AdminProductApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminProductApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteProduct(
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
|**200** | Product deleted |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAllProducts**
> Array<PickProductOrIdOrCreatedAtOrUpdatedAtOrTypeOrTitleOrSubTitleOrDescriptionOrInitialQuantityOrIconUrlOrGameId> getAllProducts()


### Example

```typescript
import {
    AdminProductApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminProductApi(configuration);

let types: Array<ProductType>; // (default to undefined)

const { status, data } = await apiInstance.getAllProducts(
    types
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **types** | **Array&lt;ProductType&gt;** |  | defaults to undefined|


### Return type

**Array<PickProductOrIdOrCreatedAtOrUpdatedAtOrTypeOrTitleOrSubTitleOrDescriptionOrInitialQuantityOrIconUrlOrGameId>**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Products fetched |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getProduct**
> PickProductOrIdOrCreatedAtOrUpdatedAtOrTypeOrTitleOrSubTitleOrDescriptionOrInitialQuantityOrIconUrlOrGameId getProduct()


### Example

```typescript
import {
    AdminProductApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminProductApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getProduct(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**PickProductOrIdOrCreatedAtOrUpdatedAtOrTypeOrTitleOrSubTitleOrDescriptionOrInitialQuantityOrIconUrlOrGameId**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Product fetched |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateProduct**
> PickProductOrIdOrCreatedAtOrUpdatedAtOrTypeOrTitleOrSubTitleOrDescriptionOrInitialQuantityOrIconUrlOrGameId updateProduct(body)


### Example

```typescript
import {
    AdminProductApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminProductApi(configuration);

let id: string; // (default to undefined)
let body: PartialCreateProductArgs; //

const { status, data } = await apiInstance.updateProduct(
    id,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **PartialCreateProductArgs**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**PickProductOrIdOrCreatedAtOrUpdatedAtOrTypeOrTitleOrSubTitleOrDescriptionOrInitialQuantityOrIconUrlOrGameId**

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Product updated |  -  |
|**0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **uploadProductImages**
> string uploadProductImages()

Uploads an image to S3 and updates the product\'s image URL in the database.

### Example

```typescript
import {
    AdminProductApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new AdminProductApi(configuration);

let id: string; //product id (default to undefined)
let imageType: string; //corresponds to the DB column name (default to undefined)
let file: File; //image to upload to S3 (default to undefined)
let replaceUrl: string; //optional url to replace (optional) (default to undefined)

const { status, data } = await apiInstance.uploadProductImages(
    id,
    imageType,
    file,
    replaceUrl
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | product id | defaults to undefined|
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

