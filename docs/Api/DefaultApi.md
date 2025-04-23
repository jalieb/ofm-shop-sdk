# OpenAPI\Client\DefaultApi

All URIs are relative to https://test.payment.stillfront.com/api/v2, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getApiV2CatalogIndex()**](DefaultApi.md#getApiV2CatalogIndex) | **GET** /catalog |  |


## `getApiV2CatalogIndex()`

```php
getApiV2CatalogIndex($game_id, $network_id, $instance_id, $player_id, $remote_address): \OpenAPI\Client\Model\GetApiV2CatalogIndex200Response
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearerAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$game_id = 56; // int
$network_id = 56; // int
$instance_id = 56; // int
$player_id = 56; // int
$remote_address = 'remote_address_example'; // string

try {
    $result = $apiInstance->getApiV2CatalogIndex($game_id, $network_id, $instance_id, $player_id, $remote_address);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->getApiV2CatalogIndex: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **game_id** | **int**|  | |
| **network_id** | **int**|  | |
| **instance_id** | **int**|  | |
| **player_id** | **int**|  | |
| **remote_address** | **string**|  | |

### Return type

[**\OpenAPI\Client\Model\GetApiV2CatalogIndex200Response**](../Model/GetApiV2CatalogIndex200Response.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
