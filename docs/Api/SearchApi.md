# Softonic\NoodleSetupApiSdk\SearchApi

All URIs are relative to *https://noodle-setup-v1.sftapi.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search**](SearchApi.md#search) | **POST** /search | Search a list of filters and returns the result


# **search**
> \Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale[] search($body)

Search a list of filters and returns the result

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Softonic\NoodleSetupApiSdk\Api\SearchApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = array(new \Softonic\NoodleSetupApiSdk\Client\Model\SearchRequest()); // \Softonic\NoodleSetupApiSdk\Client\Model\SearchRequest[] | 

try {
    $result = $apiInstance->search($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SearchApi->search: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Softonic\NoodleSetupApiSdk\Client\Model\SearchRequest[]**](../Model/SearchRequest.md)|  |

### Return type

[**\Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale[]**](../Model/ProgramPlatformLocale.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

