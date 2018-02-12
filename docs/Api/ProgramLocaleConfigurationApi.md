# Softonic\NoodleSetupApiSdk\ProgramLocaleConfigurationApi

All URIs are relative to *https://noodle-setup-v1.sftapi.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**programsIdProgramLocalesGet**](ProgramLocaleConfigurationApi.md#programsIdProgramLocalesGet) | **GET** /programs/{id_program}/locales | Finds configurations for program in all Softonic locales
[**programsIdProgramLocalesIdLocaleDelete**](ProgramLocaleConfigurationApi.md#programsIdProgramLocalesIdLocaleDelete) | **DELETE** /programs/{id_program}/locales/{id_locale} | Deletes a program configuration for a specific locale
[**programsIdProgramLocalesIdLocaleGet**](ProgramLocaleConfigurationApi.md#programsIdProgramLocalesIdLocaleGet) | **GET** /programs/{id_program}/locales/{id_locale} | Finds configurations for program and Softonic locale
[**programsIdProgramLocalesIdLocalePatch**](ProgramLocaleConfigurationApi.md#programsIdProgramLocalesIdLocalePatch) | **PATCH** /programs/{id_program}/locales/{id_locale} | Updates a program configuration for a specific locale
[**programsIdProgramLocalesIdLocalePut**](ProgramLocaleConfigurationApi.md#programsIdProgramLocalesIdLocalePut) | **PUT** /programs/{id_program}/locales/{id_locale} | Replaces a program configuration for a specific locale
[**programsIdProgramLocalesPost**](ProgramLocaleConfigurationApi.md#programsIdProgramLocalesPost) | **POST** /programs/{id_program}/locales | Creates a program configuration for a specific locale


# **programsIdProgramLocalesGet**
> \Softonic\NoodleSetupApiSdk\Client\Model\Program[] programsIdProgramLocalesGet($id_program)

Finds configurations for program in all Softonic locales



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Softonic\NoodleSetupApiSdk\Api\ProgramLocaleConfigurationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id_program = "id_program_example"; // string | Program identifier

try {
    $result = $apiInstance->programsIdProgramLocalesGet($id_program);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProgramLocaleConfigurationApi->programsIdProgramLocalesGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id_program** | [**string**](../Model/.md)| Program identifier |

### Return type

[**\Softonic\NoodleSetupApiSdk\Client\Model\Program[]**](../Model/Program.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **programsIdProgramLocalesIdLocaleDelete**
> \Softonic\NoodleSetupApiSdk\Client\Model\Program programsIdProgramLocalesIdLocaleDelete($id_program, $id_locale)

Deletes a program configuration for a specific locale

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Softonic\NoodleSetupApiSdk\Api\ProgramLocaleConfigurationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id_program = "id_program_example"; // string | Program identifier
$id_locale = "id_locale_example"; // string | Locale identifier

try {
    $result = $apiInstance->programsIdProgramLocalesIdLocaleDelete($id_program, $id_locale);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProgramLocaleConfigurationApi->programsIdProgramLocalesIdLocaleDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id_program** | [**string**](../Model/.md)| Program identifier |
 **id_locale** | **string**| Locale identifier |

### Return type

[**\Softonic\NoodleSetupApiSdk\Client\Model\Program**](../Model/Program.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **programsIdProgramLocalesIdLocaleGet**
> \Softonic\NoodleSetupApiSdk\Client\Model\Program[] programsIdProgramLocalesIdLocaleGet($id_program, $id_locale)

Finds configurations for program and Softonic locale



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Softonic\NoodleSetupApiSdk\Api\ProgramLocaleConfigurationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id_program = "id_program_example"; // string | Program identifier
$id_locale = "id_locale_example"; // string | Locale identifier

try {
    $result = $apiInstance->programsIdProgramLocalesIdLocaleGet($id_program, $id_locale);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProgramLocaleConfigurationApi->programsIdProgramLocalesIdLocaleGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id_program** | [**string**](../Model/.md)| Program identifier |
 **id_locale** | **string**| Locale identifier |

### Return type

[**\Softonic\NoodleSetupApiSdk\Client\Model\Program[]**](../Model/Program.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **programsIdProgramLocalesIdLocalePatch**
> \Softonic\NoodleSetupApiSdk\Client\Model\Program programsIdProgramLocalesIdLocalePatch($id_program, $id_locale, $body)

Updates a program configuration for a specific locale

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Softonic\NoodleSetupApiSdk\Api\ProgramLocaleConfigurationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id_program = "id_program_example"; // string | Program identifier
$id_locale = "id_locale_example"; // string | Locale identifier
$body = new \Softonic\NoodleSetupApiSdk\Client\Model\Program(); // \Softonic\NoodleSetupApiSdk\Client\Model\Program | Program locale configuration object

try {
    $result = $apiInstance->programsIdProgramLocalesIdLocalePatch($id_program, $id_locale, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProgramLocaleConfigurationApi->programsIdProgramLocalesIdLocalePatch: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id_program** | [**string**](../Model/.md)| Program identifier |
 **id_locale** | **string**| Locale identifier |
 **body** | [**\Softonic\NoodleSetupApiSdk\Client\Model\Program**](../Model/Program.md)| Program locale configuration object |

### Return type

[**\Softonic\NoodleSetupApiSdk\Client\Model\Program**](../Model/Program.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **programsIdProgramLocalesIdLocalePut**
> \Softonic\NoodleSetupApiSdk\Client\Model\Program programsIdProgramLocalesIdLocalePut($id_program, $id_locale, $body)

Replaces a program configuration for a specific locale

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Softonic\NoodleSetupApiSdk\Api\ProgramLocaleConfigurationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id_program = "id_program_example"; // string | Program identifier
$id_locale = "id_locale_example"; // string | Locale identifier
$body = new \Softonic\NoodleSetupApiSdk\Client\Model\Program(); // \Softonic\NoodleSetupApiSdk\Client\Model\Program | Program locale configuration object

try {
    $result = $apiInstance->programsIdProgramLocalesIdLocalePut($id_program, $id_locale, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProgramLocaleConfigurationApi->programsIdProgramLocalesIdLocalePut: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id_program** | [**string**](../Model/.md)| Program identifier |
 **id_locale** | **string**| Locale identifier |
 **body** | [**\Softonic\NoodleSetupApiSdk\Client\Model\Program**](../Model/Program.md)| Program locale configuration object |

### Return type

[**\Softonic\NoodleSetupApiSdk\Client\Model\Program**](../Model/Program.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **programsIdProgramLocalesPost**
> \Softonic\NoodleSetupApiSdk\Client\Model\Program programsIdProgramLocalesPost($id_program, $body)

Creates a program configuration for a specific locale

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Softonic\NoodleSetupApiSdk\Api\ProgramLocaleConfigurationApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id_program = "id_program_example"; // string | Program identifier
$body = new \Softonic\NoodleSetupApiSdk\Client\Model\Program(); // \Softonic\NoodleSetupApiSdk\Client\Model\Program | Program locale configuration object

try {
    $result = $apiInstance->programsIdProgramLocalesPost($id_program, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProgramLocaleConfigurationApi->programsIdProgramLocalesPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id_program** | [**string**](../Model/.md)| Program identifier |
 **body** | [**\Softonic\NoodleSetupApiSdk\Client\Model\Program**](../Model/Program.md)| Program locale configuration object |

### Return type

[**\Softonic\NoodleSetupApiSdk\Client\Model\Program**](../Model/Program.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

