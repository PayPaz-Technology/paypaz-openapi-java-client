# DefaultApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**allNetWork**](DefaultApi.md#allNetWork) | **GET** /t-api/openapi/v1/bc/baseConfig/allNetWork | 获取所有的netWork |
| [**allNetWork_0**](DefaultApi.md#allNetWork_0) | **GET** /t-api/openapi/v1/bc/baseConfig/allNetWork | 获取所有的netWork |
| [**serverTime**](DefaultApi.md#serverTime) | **GET** /t-api/openapi/v1/bc/baseConfig/serverTime | 获取服务器时间 |
| [**serverTime_0**](DefaultApi.md#serverTime_0) | **GET** /t-api/openapi/v1/bc/baseConfig/serverTime | 获取服务器时间 |


<a id="allNetWork"></a>
# **allNetWork**
> RListChain allNetWork()

获取所有的netWork

获取所有的netWork

### Example
```java
// Import classes:
import org.paypaz.client.ApiClient;
import org.paypaz.client.ApiException;
import org.paypaz.client.Configuration;
import org.paypaz.client.models.*;
import org.paypaz.client.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      RListChain result = apiInstance.allNetWork();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#allNetWork");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**RListChain**](RListChain.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal Server Error |  -  |

<a id="allNetWork_0"></a>
# **allNetWork_0**
> RListChain allNetWork_0()

获取所有的netWork

获取所有的netWork

### Example
```java
// Import classes:
import org.paypaz.client.ApiClient;
import org.paypaz.client.ApiException;
import org.paypaz.client.Configuration;
import org.paypaz.client.models.*;
import org.paypaz.client.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      RListChain result = apiInstance.allNetWork_0();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#allNetWork_0");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**RListChain**](RListChain.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal Server Error |  -  |

<a id="serverTime"></a>
# **serverTime**
> RLong serverTime()

获取服务器时间

获取服务器时间

### Example
```java
// Import classes:
import org.paypaz.client.ApiClient;
import org.paypaz.client.ApiException;
import org.paypaz.client.Configuration;
import org.paypaz.client.models.*;
import org.paypaz.client.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      RLong result = apiInstance.serverTime();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#serverTime");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**RLong**](RLong.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal Server Error |  -  |

<a id="serverTime_0"></a>
# **serverTime_0**
> RLong serverTime_0()

获取服务器时间

获取服务器时间

### Example
```java
// Import classes:
import org.paypaz.client.ApiClient;
import org.paypaz.client.ApiException;
import org.paypaz.client.Configuration;
import org.paypaz.client.models.*;
import org.paypaz.client.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      RLong result = apiInstance.serverTime_0();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#serverTime_0");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**RLong**](RLong.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | Unauthorized |  -  |
| **500** | Internal Server Error |  -  |

