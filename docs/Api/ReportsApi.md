# Swagger\Client\ReportsApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ordersGET**](ReportsApi.md#ordersget) | **GET** /api/merchant/v1/reports/orders/{orderId} | 
[**ordersPOST**](ReportsApi.md#orderspost) | **POST** /api/merchant/v1/reports/orders | 

# **ordersGET**
> ordersGET($order_id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ReportsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$order_id = "order_id_example"; // string | 

try {
    $apiInstance->ordersGET($order_id);
} catch (Exception $e) {
    echo 'Exception when calling ReportsApi->ordersGET: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order_id** | **string**|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **ordersPOST**
> ordersPOST($body)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ReportsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Swagger\Client\Model\map(); // map[string,null] | 

try {
    $apiInstance->ordersPOST($body);
} catch (Exception $e) {
    echo 'Exception when calling ReportsApi->ordersPOST: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**map[string,null]**](../Model/map.md)|  | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

