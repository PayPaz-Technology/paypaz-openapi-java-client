# PaypazBrokerOpenApiApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createWithdrawal**](PaypazBrokerOpenApiApi.md#createWithdrawal) | **POST** /t-api/broker-openapi/v1/op/openapi/createWithdrawal | 根据UID发起提币  为指定子用户创建提币订单
[**createWithdrawal_0**](PaypazBrokerOpenApiApi.md#createWithdrawal_0) | **POST** /t-api/broker-openapi/v1/op/openapi/createWithdrawal | 根据UID发起提币  为指定子用户创建提币订单
[**getDepositAddress**](PaypazBrokerOpenApiApi.md#getDepositAddress) | **POST** /t-api/broker-openapi/v1/op/openapi/depositAddress | 获取或创建充值地址  为指定子用户和币种获取充值地址，如果该币种地址不存在，则创建新地址
[**getDepositAddress_0**](PaypazBrokerOpenApiApi.md#getDepositAddress_0) | **POST** /t-api/broker-openapi/v1/op/openapi/depositAddress | 获取或创建充值地址  为指定子用户和币种获取充值地址，如果该币种地址不存在，则创建新地址
[**queryBrokerAssets**](PaypazBrokerOpenApiApi.md#queryBrokerAssets) | **GET** /t-api/broker-openapi/v1/op/openapi/assets | 查询Broker下所有资产信息  查询当前OpenAPI用户下指定币种或所有币种的资产信息
[**queryBrokerAssets_0**](PaypazBrokerOpenApiApi.md#queryBrokerAssets_0) | **GET** /t-api/broker-openapi/v1/op/openapi/assets | 查询Broker下所有资产信息  查询当前OpenAPI用户下指定币种或所有币种的资产信息
[**queryDepositOrders**](PaypazBrokerOpenApiApi.md#queryDepositOrders) | **POST** /t-api/broker-openapi/v1/op/openapi/depositOrders | 分页查询充值订单  根据条件查询充值订单列表，支持分页、时间范围、币种、钱包地址等筛选条件
[**queryDepositOrders_0**](PaypazBrokerOpenApiApi.md#queryDepositOrders_0) | **POST** /t-api/broker-openapi/v1/op/openapi/depositOrders | 分页查询充值订单  根据条件查询充值订单列表，支持分页、时间范围、币种、钱包地址等筛选条件
[**queryWithdrawalOrders**](PaypazBrokerOpenApiApi.md#queryWithdrawalOrders) | **POST** /t-api/broker-openapi/v1/op/openapi/withdrawalOrders | 根据subUID、地址、订单号查询提币订单  分页查询指定条件下的提币订单列表
[**queryWithdrawalOrders_0**](PaypazBrokerOpenApiApi.md#queryWithdrawalOrders_0) | **POST** /t-api/broker-openapi/v1/op/openapi/withdrawalOrders | 根据subUID、地址、订单号查询提币订单  分页查询指定条件下的提币订单列表
[**withdrawalOrderInfo**](PaypazBrokerOpenApiApi.md#withdrawalOrderInfo) | **GET** /t-api/broker-openapi/v1/op/openapi/withdrawalOrderInfo | 查询提币订单详情  根据客户端提币订单ID查询提币订单详细信息
[**withdrawalOrderInfo_0**](PaypazBrokerOpenApiApi.md#withdrawalOrderInfo_0) | **GET** /t-api/broker-openapi/v1/op/openapi/withdrawalOrderInfo | 查询提币订单详情  根据客户端提币订单ID查询提币订单详细信息


<a name="createWithdrawal"></a>
# **createWithdrawal**
> RWithdrawalOrderOpenApiVo createWithdrawal(createWithdrawalRequest)

根据UID发起提币  为指定子用户创建提币订单

根据UID发起提币  为指定子用户创建提币订单

### Example
```java
// Import classes:
import org.paypaz.client.ApiClient;
import org.paypaz.client.ApiException;
import org.paypaz.client.Configuration;
import org.paypaz.client.models.*;
import org.paypaz.client.api.PaypazBrokerOpenApiApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    PaypazBrokerOpenApiApi apiInstance = new PaypazBrokerOpenApiApi(defaultClient);
    CreateWithdrawalRequest createWithdrawalRequest = new CreateWithdrawalRequest(); // CreateWithdrawalRequest | 
    try {
      RWithdrawalOrderOpenApiVo result = apiInstance.createWithdrawal(createWithdrawalRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling PaypazBrokerOpenApiApi#createWithdrawal");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createWithdrawalRequest** | [**CreateWithdrawalRequest**](CreateWithdrawalRequest.md)|  | [optional]

### Return type

[**RWithdrawalOrderOpenApiVo**](RWithdrawalOrderOpenApiVo.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 提币订单ID |  -  |
**401** | Unauthorized |  -  |
**500** | Internal Server Error |  -  |

<a name="createWithdrawal_0"></a>
# **createWithdrawal_0**
> RWithdrawalOrderOpenApiVo createWithdrawal_0(createWithdrawalRequest)

根据UID发起提币  为指定子用户创建提币订单

根据UID发起提币  为指定子用户创建提币订单

### Example
```java
// Import classes:
import org.paypaz.client.ApiClient;
import org.paypaz.client.ApiException;
import org.paypaz.client.Configuration;
import org.paypaz.client.models.*;
import org.paypaz.client.api.PaypazBrokerOpenApiApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    PaypazBrokerOpenApiApi apiInstance = new PaypazBrokerOpenApiApi(defaultClient);
    CreateWithdrawalRequest createWithdrawalRequest = new CreateWithdrawalRequest(); // CreateWithdrawalRequest | 
    try {
      RWithdrawalOrderOpenApiVo result = apiInstance.createWithdrawal_0(createWithdrawalRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling PaypazBrokerOpenApiApi#createWithdrawal_0");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createWithdrawalRequest** | [**CreateWithdrawalRequest**](CreateWithdrawalRequest.md)|  | [optional]

### Return type

[**RWithdrawalOrderOpenApiVo**](RWithdrawalOrderOpenApiVo.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 提币订单ID |  -  |
**401** | Unauthorized |  -  |
**500** | Internal Server Error |  -  |

<a name="getDepositAddress"></a>
# **getDepositAddress**
> RSubWalletAddressOpenApiVo getDepositAddress(getDepositAddressRequest)

获取或创建充值地址  为指定子用户和币种获取充值地址，如果该币种地址不存在，则创建新地址

获取或创建充值地址  为指定子用户和币种获取充值地址，如果该币种地址不存在，则创建新地址

### Example
```java
// Import classes:
import org.paypaz.client.ApiClient;
import org.paypaz.client.ApiException;
import org.paypaz.client.Configuration;
import org.paypaz.client.models.*;
import org.paypaz.client.api.PaypazBrokerOpenApiApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    PaypazBrokerOpenApiApi apiInstance = new PaypazBrokerOpenApiApi(defaultClient);
    GetDepositAddressRequest getDepositAddressRequest = new GetDepositAddressRequest(); // GetDepositAddressRequest | 
    try {
      RSubWalletAddressOpenApiVo result = apiInstance.getDepositAddress(getDepositAddressRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling PaypazBrokerOpenApiApi#getDepositAddress");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **getDepositAddressRequest** | [**GetDepositAddressRequest**](GetDepositAddressRequest.md)|  | [optional]

### Return type

[**RSubWalletAddressOpenApiVo**](RSubWalletAddressOpenApiVo.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 包含充值地址信息的响应对象，数据为{@link SubWalletAddressOpenApiVO SubWalletAddressOpenApiVO} |  -  |
**401** | Unauthorized |  -  |
**500** | Internal Server Error |  -  |

<a name="getDepositAddress_0"></a>
# **getDepositAddress_0**
> RSubWalletAddressOpenApiVo getDepositAddress_0(getDepositAddressRequest)

获取或创建充值地址  为指定子用户和币种获取充值地址，如果该币种地址不存在，则创建新地址

获取或创建充值地址  为指定子用户和币种获取充值地址，如果该币种地址不存在，则创建新地址

### Example
```java
// Import classes:
import org.paypaz.client.ApiClient;
import org.paypaz.client.ApiException;
import org.paypaz.client.Configuration;
import org.paypaz.client.models.*;
import org.paypaz.client.api.PaypazBrokerOpenApiApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    PaypazBrokerOpenApiApi apiInstance = new PaypazBrokerOpenApiApi(defaultClient);
    GetDepositAddressRequest getDepositAddressRequest = new GetDepositAddressRequest(); // GetDepositAddressRequest | 
    try {
      RSubWalletAddressOpenApiVo result = apiInstance.getDepositAddress_0(getDepositAddressRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling PaypazBrokerOpenApiApi#getDepositAddress_0");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **getDepositAddressRequest** | [**GetDepositAddressRequest**](GetDepositAddressRequest.md)|  | [optional]

### Return type

[**RSubWalletAddressOpenApiVo**](RSubWalletAddressOpenApiVo.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 包含充值地址信息的响应对象，数据为{@link SubWalletAddressOpenApiVO SubWalletAddressOpenApiVO} |  -  |
**401** | Unauthorized |  -  |
**500** | Internal Server Error |  -  |

<a name="queryBrokerAssets"></a>
# **queryBrokerAssets**
> RListBalanceOpenApiVo queryBrokerAssets(tokenId)

查询Broker下所有资产信息  查询当前OpenAPI用户下指定币种或所有币种的资产信息

查询Broker下所有资产信息  查询当前OpenAPI用户下指定币种或所有币种的资产信息

### Example
```java
// Import classes:
import org.paypaz.client.ApiClient;
import org.paypaz.client.ApiException;
import org.paypaz.client.Configuration;
import org.paypaz.client.models.*;
import org.paypaz.client.api.PaypazBrokerOpenApiApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    PaypazBrokerOpenApiApi apiInstance = new PaypazBrokerOpenApiApi(defaultClient);
    String tokenId = "tokenId_example"; // String | 可选参数，币种ID。如果提供，则只返回该币种的资产信息；如果为null，则返回所有币种资产信息
    try {
      RListBalanceOpenApiVo result = apiInstance.queryBrokerAssets(tokenId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling PaypazBrokerOpenApiApi#queryBrokerAssets");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tokenId** | **String**| 可选参数，币种ID。如果提供，则只返回该币种的资产信息；如果为null，则返回所有币种资产信息 | [optional]

### Return type

[**RListBalanceOpenApiVo**](RListBalanceOpenApiVo.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 包含资产信息的响应对象，数据为{@link BalanceOpenApiVO BalanceOpenApiVO}列表 |  -  |
**401** | Unauthorized |  -  |
**500** | Internal Server Error |  -  |

<a name="queryBrokerAssets_0"></a>
# **queryBrokerAssets_0**
> RListBalanceOpenApiVo queryBrokerAssets_0(tokenId)

查询Broker下所有资产信息  查询当前OpenAPI用户下指定币种或所有币种的资产信息

查询Broker下所有资产信息  查询当前OpenAPI用户下指定币种或所有币种的资产信息

### Example
```java
// Import classes:
import org.paypaz.client.ApiClient;
import org.paypaz.client.ApiException;
import org.paypaz.client.Configuration;
import org.paypaz.client.models.*;
import org.paypaz.client.api.PaypazBrokerOpenApiApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    PaypazBrokerOpenApiApi apiInstance = new PaypazBrokerOpenApiApi(defaultClient);
    String tokenId = "tokenId_example"; // String | 可选参数，币种ID。如果提供，则只返回该币种的资产信息；如果为null，则返回所有币种资产信息
    try {
      RListBalanceOpenApiVo result = apiInstance.queryBrokerAssets_0(tokenId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling PaypazBrokerOpenApiApi#queryBrokerAssets_0");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tokenId** | **String**| 可选参数，币种ID。如果提供，则只返回该币种的资产信息；如果为null，则返回所有币种资产信息 | [optional]

### Return type

[**RListBalanceOpenApiVo**](RListBalanceOpenApiVo.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 包含资产信息的响应对象，数据为{@link BalanceOpenApiVO BalanceOpenApiVO}列表 |  -  |
**401** | Unauthorized |  -  |
**500** | Internal Server Error |  -  |

<a name="queryDepositOrders"></a>
# **queryDepositOrders**
> RPageDepositOrderOpenApiVo queryDepositOrders(queryDepositOrderRequest)

分页查询充值订单  根据条件查询充值订单列表，支持分页、时间范围、币种、钱包地址等筛选条件

分页查询充值订单  根据条件查询充值订单列表，支持分页、时间范围、币种、钱包地址等筛选条件

### Example
```java
// Import classes:
import org.paypaz.client.ApiClient;
import org.paypaz.client.ApiException;
import org.paypaz.client.Configuration;
import org.paypaz.client.models.*;
import org.paypaz.client.api.PaypazBrokerOpenApiApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    PaypazBrokerOpenApiApi apiInstance = new PaypazBrokerOpenApiApi(defaultClient);
    QueryDepositOrderRequest queryDepositOrderRequest = new QueryDepositOrderRequest(); // QueryDepositOrderRequest | 
    try {
      RPageDepositOrderOpenApiVo result = apiInstance.queryDepositOrders(queryDepositOrderRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling PaypazBrokerOpenApiApi#queryDepositOrders");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **queryDepositOrderRequest** | [**QueryDepositOrderRequest**](QueryDepositOrderRequest.md)|  | [optional]

### Return type

[**RPageDepositOrderOpenApiVo**](RPageDepositOrderOpenApiVo.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 包含充值订单分页数据的响应对象，数据为{@link DepositOrderOpenApiVO DepositOrderOpenApiVO}分页列表 |  -  |
**401** | Unauthorized |  -  |
**500** | Internal Server Error |  -  |

<a name="queryDepositOrders_0"></a>
# **queryDepositOrders_0**
> RPageDepositOrderOpenApiVo queryDepositOrders_0(queryDepositOrderRequest)

分页查询充值订单  根据条件查询充值订单列表，支持分页、时间范围、币种、钱包地址等筛选条件

分页查询充值订单  根据条件查询充值订单列表，支持分页、时间范围、币种、钱包地址等筛选条件

### Example
```java
// Import classes:
import org.paypaz.client.ApiClient;
import org.paypaz.client.ApiException;
import org.paypaz.client.Configuration;
import org.paypaz.client.models.*;
import org.paypaz.client.api.PaypazBrokerOpenApiApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    PaypazBrokerOpenApiApi apiInstance = new PaypazBrokerOpenApiApi(defaultClient);
    QueryDepositOrderRequest queryDepositOrderRequest = new QueryDepositOrderRequest(); // QueryDepositOrderRequest | 
    try {
      RPageDepositOrderOpenApiVo result = apiInstance.queryDepositOrders_0(queryDepositOrderRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling PaypazBrokerOpenApiApi#queryDepositOrders_0");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **queryDepositOrderRequest** | [**QueryDepositOrderRequest**](QueryDepositOrderRequest.md)|  | [optional]

### Return type

[**RPageDepositOrderOpenApiVo**](RPageDepositOrderOpenApiVo.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 包含充值订单分页数据的响应对象，数据为{@link DepositOrderOpenApiVO DepositOrderOpenApiVO}分页列表 |  -  |
**401** | Unauthorized |  -  |
**500** | Internal Server Error |  -  |

<a name="queryWithdrawalOrders"></a>
# **queryWithdrawalOrders**
> RPageWithdrawalOrderOpenApiVo queryWithdrawalOrders(queryWithdrawalOrderRequest)

根据subUID、地址、订单号查询提币订单  分页查询指定条件下的提币订单列表

根据subUID、地址、订单号查询提币订单  分页查询指定条件下的提币订单列表

### Example
```java
// Import classes:
import org.paypaz.client.ApiClient;
import org.paypaz.client.ApiException;
import org.paypaz.client.Configuration;
import org.paypaz.client.models.*;
import org.paypaz.client.api.PaypazBrokerOpenApiApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    PaypazBrokerOpenApiApi apiInstance = new PaypazBrokerOpenApiApi(defaultClient);
    QueryWithdrawalOrderRequest queryWithdrawalOrderRequest = new QueryWithdrawalOrderRequest(); // QueryWithdrawalOrderRequest | 
    try {
      RPageWithdrawalOrderOpenApiVo result = apiInstance.queryWithdrawalOrders(queryWithdrawalOrderRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling PaypazBrokerOpenApiApi#queryWithdrawalOrders");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **queryWithdrawalOrderRequest** | [**QueryWithdrawalOrderRequest**](QueryWithdrawalOrderRequest.md)|  | [optional]

### Return type

[**RPageWithdrawalOrderOpenApiVo**](RPageWithdrawalOrderOpenApiVo.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 提币订单分页列表 |  -  |
**401** | Unauthorized |  -  |
**500** | Internal Server Error |  -  |

<a name="queryWithdrawalOrders_0"></a>
# **queryWithdrawalOrders_0**
> RPageWithdrawalOrderOpenApiVo queryWithdrawalOrders_0(queryWithdrawalOrderRequest)

根据subUID、地址、订单号查询提币订单  分页查询指定条件下的提币订单列表

根据subUID、地址、订单号查询提币订单  分页查询指定条件下的提币订单列表

### Example
```java
// Import classes:
import org.paypaz.client.ApiClient;
import org.paypaz.client.ApiException;
import org.paypaz.client.Configuration;
import org.paypaz.client.models.*;
import org.paypaz.client.api.PaypazBrokerOpenApiApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    PaypazBrokerOpenApiApi apiInstance = new PaypazBrokerOpenApiApi(defaultClient);
    QueryWithdrawalOrderRequest queryWithdrawalOrderRequest = new QueryWithdrawalOrderRequest(); // QueryWithdrawalOrderRequest | 
    try {
      RPageWithdrawalOrderOpenApiVo result = apiInstance.queryWithdrawalOrders_0(queryWithdrawalOrderRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling PaypazBrokerOpenApiApi#queryWithdrawalOrders_0");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **queryWithdrawalOrderRequest** | [**QueryWithdrawalOrderRequest**](QueryWithdrawalOrderRequest.md)|  | [optional]

### Return type

[**RPageWithdrawalOrderOpenApiVo**](RPageWithdrawalOrderOpenApiVo.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 提币订单分页列表 |  -  |
**401** | Unauthorized |  -  |
**500** | Internal Server Error |  -  |

<a name="withdrawalOrderInfo"></a>
# **withdrawalOrderInfo**
> RWithdrawalOrderOpenApiVo withdrawalOrderInfo(clientWithdrawalId)

查询提币订单详情  根据客户端提币订单ID查询提币订单详细信息

查询提币订单详情  根据客户端提币订单ID查询提币订单详细信息

### Example
```java
// Import classes:
import org.paypaz.client.ApiClient;
import org.paypaz.client.ApiException;
import org.paypaz.client.Configuration;
import org.paypaz.client.models.*;
import org.paypaz.client.api.PaypazBrokerOpenApiApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    PaypazBrokerOpenApiApi apiInstance = new PaypazBrokerOpenApiApi(defaultClient);
    String clientWithdrawalId = "clientWithdrawalId_example"; // String | 客户端提币订单ID
    try {
      RWithdrawalOrderOpenApiVo result = apiInstance.withdrawalOrderInfo(clientWithdrawalId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling PaypazBrokerOpenApiApi#withdrawalOrderInfo");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **clientWithdrawalId** | **String**| 客户端提币订单ID |

### Return type

[**RWithdrawalOrderOpenApiVo**](RWithdrawalOrderOpenApiVo.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 提币订单详情 |  -  |
**401** | Unauthorized |  -  |
**500** | Internal Server Error |  -  |

<a name="withdrawalOrderInfo_0"></a>
# **withdrawalOrderInfo_0**
> RWithdrawalOrderOpenApiVo withdrawalOrderInfo_0(clientWithdrawalId)

查询提币订单详情  根据客户端提币订单ID查询提币订单详细信息

查询提币订单详情  根据客户端提币订单ID查询提币订单详细信息

### Example
```java
// Import classes:
import org.paypaz.client.ApiClient;
import org.paypaz.client.ApiException;
import org.paypaz.client.Configuration;
import org.paypaz.client.models.*;
import org.paypaz.client.api.PaypazBrokerOpenApiApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    PaypazBrokerOpenApiApi apiInstance = new PaypazBrokerOpenApiApi(defaultClient);
    String clientWithdrawalId = "clientWithdrawalId_example"; // String | 客户端提币订单ID
    try {
      RWithdrawalOrderOpenApiVo result = apiInstance.withdrawalOrderInfo_0(clientWithdrawalId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling PaypazBrokerOpenApiApi#withdrawalOrderInfo_0");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **clientWithdrawalId** | **String**| 客户端提币订单ID |

### Return type

[**RWithdrawalOrderOpenApiVo**](RWithdrawalOrderOpenApiVo.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 提币订单详情 |  -  |
**401** | Unauthorized |  -  |
**500** | Internal Server Error |  -  |

