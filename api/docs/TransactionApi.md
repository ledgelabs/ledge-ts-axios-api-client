# TransactionApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getAllTransactions**](#getalltransactions) | **GET** /transaction | |

# **getAllTransactions**
> PaginatedTransactionDetailed getAllTransactions()


### Example

```typescript
import {
    TransactionApi,
    Configuration
} from './api';

const configuration = new Configuration();
const apiInstance = new TransactionApi(configuration);

let sellProductType: Array<ProductType>; // (optional) (default to undefined)
let sellProductId: string; // (optional) (default to undefined)
let page: number; // (optional) (default to 0)
let limit: number; // (optional) (default to 10)

const { status, data } = await apiInstance.getAllTransactions(
    sellProductType,
    sellProductId,
    page,
    limit
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sellProductType** | **Array&lt;ProductType&gt;** |  | (optional) defaults to undefined|
| **sellProductId** | [**string**] |  | (optional) defaults to undefined|
| **page** | [**number**] |  | (optional) defaults to 0|
| **limit** | [**number**] |  | (optional) defaults to 10|


### Return type

**PaginatedTransactionDetailed**

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

