# OpenAPI\Client\ManageServiceApi

All URIs are relative to https://api.beget.com, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**manageServiceCreateImage()**](ManageServiceApi.md#manageServiceCreateImage) | **POST** /v1/image |  |
| [**manageServiceDeleteImage()**](ManageServiceApi.md#manageServiceDeleteImage) | **DELETE** /v1/image/{id} |  |
| [**manageServiceGetCalculation()**](ManageServiceApi.md#manageServiceGetCalculation) | **GET** /v1/image/calculation |  |
| [**manageServiceGetDownloadLink()**](ManageServiceApi.md#manageServiceGetDownloadLink) | **GET** /v1/image/{id}/link |  |
| [**manageServiceGetList()**](ManageServiceApi.md#manageServiceGetList) | **GET** /v1/image |  |
| [**manageServiceGetRegionList()**](ManageServiceApi.md#manageServiceGetRegionList) | **GET** /v1/image/region |  |
| [**manageServiceRestoreImage()**](ManageServiceApi.md#manageServiceRestoreImage) | **POST** /v1/image/{id}/restore |  |
| [**manageServiceUpdateImage()**](ManageServiceApi.md#manageServiceUpdateImage) | **PUT** /v1/image/{id} |  |


## `manageServiceCreateImage()`

```php
manageServiceCreateImage($image_create_image_request): \OpenAPI\Client\Model\ImageCreateImageResponse
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearerAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\ManageServiceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$image_create_image_request = new \OpenAPI\Client\Model\ImageCreateImageRequest(); // \OpenAPI\Client\Model\ImageCreateImageRequest

try {
    $result = $apiInstance->manageServiceCreateImage($image_create_image_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManageServiceApi->manageServiceCreateImage: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **image_create_image_request** | [**\OpenAPI\Client\Model\ImageCreateImageRequest**](../Model/ImageCreateImageRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\ImageCreateImageResponse**](../Model/ImageCreateImageResponse.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `manageServiceDeleteImage()`

```php
manageServiceDeleteImage($id): \OpenAPI\Client\Model\ImageDeleteImageResponse
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearerAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\ManageServiceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string

try {
    $result = $apiInstance->manageServiceDeleteImage($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManageServiceApi->manageServiceDeleteImage: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |

### Return type

[**\OpenAPI\Client\Model\ImageDeleteImageResponse**](../Model/ImageDeleteImageResponse.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `manageServiceGetCalculation()`

```php
manageServiceGetCalculation($file_size, $link, $vps_id): \OpenAPI\Client\Model\ImageGetCalculationResponse
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearerAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\ManageServiceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$file_size = 'file_size_example'; // string
$link = 'link_example'; // string
$vps_id = 'vps_id_example'; // string

try {
    $result = $apiInstance->manageServiceGetCalculation($file_size, $link, $vps_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManageServiceApi->manageServiceGetCalculation: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **file_size** | **string**|  | [optional] |
| **link** | **string**|  | [optional] |
| **vps_id** | **string**|  | [optional] |

### Return type

[**\OpenAPI\Client\Model\ImageGetCalculationResponse**](../Model/ImageGetCalculationResponse.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `manageServiceGetDownloadLink()`

```php
manageServiceGetDownloadLink($id): \OpenAPI\Client\Model\ImageGetDownloadLinkResponse
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearerAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\ManageServiceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string

try {
    $result = $apiInstance->manageServiceGetDownloadLink($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManageServiceApi->manageServiceGetDownloadLink: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |

### Return type

[**\OpenAPI\Client\Model\ImageGetDownloadLinkResponse**](../Model/ImageGetDownloadLinkResponse.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `manageServiceGetList()`

```php
manageServiceGetList(): \OpenAPI\Client\Model\ImageGetListResponse
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearerAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\ManageServiceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->manageServiceGetList();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManageServiceApi->manageServiceGetList: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\OpenAPI\Client\Model\ImageGetListResponse**](../Model/ImageGetListResponse.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `manageServiceGetRegionList()`

```php
manageServiceGetRegionList(): \OpenAPI\Client\Model\ImageGetRegionListResponse
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearerAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\ManageServiceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->manageServiceGetRegionList();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManageServiceApi->manageServiceGetRegionList: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\OpenAPI\Client\Model\ImageGetRegionListResponse**](../Model/ImageGetRegionListResponse.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `manageServiceRestoreImage()`

```php
manageServiceRestoreImage($id, $image_restore_image_request): \OpenAPI\Client\Model\ImageRestoreImageResponse
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearerAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\ManageServiceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$image_restore_image_request = new \OpenAPI\Client\Model\ImageRestoreImageRequest(); // \OpenAPI\Client\Model\ImageRestoreImageRequest

try {
    $result = $apiInstance->manageServiceRestoreImage($id, $image_restore_image_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManageServiceApi->manageServiceRestoreImage: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **image_restore_image_request** | [**\OpenAPI\Client\Model\ImageRestoreImageRequest**](../Model/ImageRestoreImageRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\ImageRestoreImageResponse**](../Model/ImageRestoreImageResponse.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `manageServiceUpdateImage()`

```php
manageServiceUpdateImage($id, $image_update_image_request): \OpenAPI\Client\Model\ImageUpdateImageResponse
```



### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearerAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\ManageServiceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$image_update_image_request = new \OpenAPI\Client\Model\ImageUpdateImageRequest(); // \OpenAPI\Client\Model\ImageUpdateImageRequest

try {
    $result = $apiInstance->manageServiceUpdateImage($id, $image_update_image_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManageServiceApi->manageServiceUpdateImage: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **image_update_image_request** | [**\OpenAPI\Client\Model\ImageUpdateImageRequest**](../Model/ImageUpdateImageRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\ImageUpdateImageResponse**](../Model/ImageUpdateImageResponse.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
