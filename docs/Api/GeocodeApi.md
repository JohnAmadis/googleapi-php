# GoogleApi\Client\GeocodeApi

All URIs are relative to *https://maps.googleapis.com/maps/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getInformation**](GeocodeApi.md#getInformation) | **GET** /geocode/json | Gets Geo-Information about the specified place


# **getInformation**
> \GoogleApi\Client\Model\InlineResponse200 getInformation($address, $latlng, $language, $key)

Gets Geo-Information about the specified place

Converts address to latlng and vice versa

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new GoogleApi\Client\Api\GeocodeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$address = "address_example"; // string | Address to convert into the latlng
$latlng = "latlng_example"; // string | LatLng to convert into the address
$language = "language_example"; // string | Language to return the results in
$key = "key_example"; // string | Security key to use for authorization

try {
    $result = $apiInstance->getInformation($address, $latlng, $language, $key);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling GeocodeApi->getInformation: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **address** | **string**| Address to convert into the latlng | [optional]
 **latlng** | **string**| LatLng to convert into the address | [optional]
 **language** | **string**| Language to return the results in | [optional]
 **key** | **string**| Security key to use for authorization | [optional]

### Return type

[**\GoogleApi\Client\Model\InlineResponse200**](../Model/InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

