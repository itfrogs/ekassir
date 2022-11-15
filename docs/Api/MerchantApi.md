# Swagger\Client\MerchantApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**petition**](MerchantApi.md#petition) | **POST** /api/merchant/v1/petition/{qrcId} | 
[**qRCodeGet**](MerchantApi.md#qrcodeget) | **GET** /api/merchant/v1/qrc-data/{qrcId}/payload | Get QR-code payload
[**qRCodePost**](MerchantApi.md#qrcodepost) | **POST** /api/merchant/v1/qrc-data | Register QR-code data
[**qRCodePost_0**](MerchantApi.md#qrcodepost_0) | **PUT** /api/merchant/v1/qrc-status | Get QR-codes statuses

# **petition**
> petition($qrc_id, $body)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\MerchantApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$qrc_id = "qrc_id_example"; // string | 
$body = new \Swagger\Client\Model\map(); // map[string,null] | 

try {
    $apiInstance->petition($qrc_id, $body);
} catch (Exception $e) {
    echo 'Exception when calling MerchantApi->petition: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **qrc_id** | **string**|  |
 **body** | [**map[string,null]**](../Model/map.md)|  | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/_*+json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **qRCodeGet**
> \Swagger\Client\Model\QrcPayloadResultOk qRCodeGet($qrc_id, $media_type, $width, $height)

Get QR-code payload

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\MerchantApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$qrc_id = "qrc_id_example"; // string | 
$media_type = new \Swagger\Client\Model\MediaType(); // \Swagger\Client\Model\MediaType | 
$width = 300; // int | 
$height = 300; // int | 

try {
    $result = $apiInstance->qRCodeGet($qrc_id, $media_type, $width, $height);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MerchantApi->qRCodeGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **qrc_id** | **string**|  |
 **media_type** | [**\Swagger\Client\Model\MediaType**](../Model/.md)|  | [optional]
 **width** | **int**|  | [optional] [default to 300]
 **height** | **int**|  | [optional] [default to 300]

### Return type

[**\Swagger\Client\Model\QrcPayloadResultOk**](../Model/QrcPayloadResultOk.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, application/jose

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **qRCodePost**
> \Swagger\Client\Model\QrcDataResultOk qRCodePost($body, $media_type, $width, $height)

Register QR-code data

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\MerchantApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Swagger\Client\Model\map(); // map[string,null] | 
$media_type = new \Swagger\Client\Model\MediaType(); // \Swagger\Client\Model\MediaType | 
$width = 300; // int | 
$height = 300; // int | 

try {
    $result = $apiInstance->qRCodePost($body, $media_type, $width, $height);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MerchantApi->qRCodePost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**map[string,null]**](../Model/map.md)|  |
 **media_type** | [**\Swagger\Client\Model\MediaType**](../Model/.md)|  | [optional]
 **width** | **int**|  | [optional] [default to 300]
 **height** | **int**|  | [optional] [default to 300]

### Return type

[**\Swagger\Client\Model\QrcDataResultOk**](../Model/QrcDataResultOk.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/_*+json
 - **Accept**: application/json, application/jose

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **qRCodePost_0**
> \Swagger\Client\Model\QrcStatusResultOk qRCodePost_0($body)

Get QR-codes statuses

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\MerchantApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Swagger\Client\Model\map(); // map[string,null] | 

try {
    $result = $apiInstance->qRCodePost_0($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MerchantApi->qRCodePost_0: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**map[string,null]**](../Model/map.md)|  |

### Return type

[**\Swagger\Client\Model\QrcStatusResultOk**](../Model/QrcStatusResultOk.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/json, text/json, application/_*+json
 - **Accept**: application/json, application/jose

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

