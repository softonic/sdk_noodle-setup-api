# Softonic\NoodleSetupApiSdk\ProgramsPlatformsLocalesApi

All URIs are relative to *https://noodle-setup-v1.sftapi.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createProgramPlatformLocale**](ProgramsPlatformsLocalesApi.md#createProgramPlatformLocale) | **POST** /programs/{id_program}/platforms/{id_platform}/locales | Creates a program configuration for a specific platform and locale
[**deleteProgramPlatformLocale**](ProgramsPlatformsLocalesApi.md#deleteProgramPlatformLocale) | **DELETE** /programs/{id_program}/platforms/{id_platform}/locales/{id_locale} | Deletes a program configuration for a specific platform and locale
[**findProgramPlatformLocale**](ProgramsPlatformsLocalesApi.md#findProgramPlatformLocale) | **GET** /programs/{id_program}/platforms/{id_platform}/locales | Finds a program configuration for a specific platform for all locales
[**readProgramPlatformLocale**](ProgramsPlatformsLocalesApi.md#readProgramPlatformLocale) | **GET** /programs/{id_program}/platforms/{id_platform}/locales/{id_locale} | Reads a program configuration for a specific platform and locale
[**replaceProgramPlatformLocale**](ProgramsPlatformsLocalesApi.md#replaceProgramPlatformLocale) | **PUT** /programs/{id_program}/platforms/{id_platform}/locales/{id_locale} | Replaces a program configuration for a specific platform and locale
[**updateProgramPlatformLocale**](ProgramsPlatformsLocalesApi.md#updateProgramPlatformLocale) | **PATCH** /programs/{id_program}/platforms/{id_platform}/locales/{id_locale} | Updates a program configuration for a specific platform and locale


# **createProgramPlatformLocale**
> \Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale createProgramPlatformLocale($id_program, $id_platform, $body)

Creates a program configuration for a specific platform and locale

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Softonic\NoodleSetupApiSdk\Api\ProgramsPlatformsLocalesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id_program = "id_program_example"; // string | Program identifier
$id_platform = "id_platform_example"; // string | Platform identifier
$body = new \Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale(); // \Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale | 

try {
    $result = $apiInstance->createProgramPlatformLocale($id_program, $id_platform, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProgramsPlatformsLocalesApi->createProgramPlatformLocale: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id_program** | [**string**](../Model/.md)| Program identifier |
 **id_platform** | **string**| Platform identifier |
 **body** | [**\Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale**](../Model/ProgramPlatformLocale.md)|  |

### Return type

[**\Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale**](../Model/ProgramPlatformLocale.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteProgramPlatformLocale**
> \Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale deleteProgramPlatformLocale($id_program, $id_platform, $id_locale)

Deletes a program configuration for a specific platform and locale

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Softonic\NoodleSetupApiSdk\Api\ProgramsPlatformsLocalesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id_program = "id_program_example"; // string | Program identifier
$id_platform = "id_platform_example"; // string | Platform identifier
$id_locale = "id_locale_example"; // string | Locale identifier

try {
    $result = $apiInstance->deleteProgramPlatformLocale($id_program, $id_platform, $id_locale);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProgramsPlatformsLocalesApi->deleteProgramPlatformLocale: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id_program** | [**string**](../Model/.md)| Program identifier |
 **id_platform** | **string**| Platform identifier |
 **id_locale** | **string**| Locale identifier |

### Return type

[**\Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale**](../Model/ProgramPlatformLocale.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **findProgramPlatformLocale**
> \Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale[] findProgramPlatformLocale($id_program, $id_platform)

Finds a program configuration for a specific platform for all locales



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Softonic\NoodleSetupApiSdk\Api\ProgramsPlatformsLocalesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id_program = "id_program_example"; // string | Program identifier
$id_platform = "id_platform_example"; // string | Platform identifier

try {
    $result = $apiInstance->findProgramPlatformLocale($id_program, $id_platform);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProgramsPlatformsLocalesApi->findProgramPlatformLocale: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id_program** | [**string**](../Model/.md)| Program identifier |
 **id_platform** | **string**| Platform identifier |

### Return type

[**\Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale[]**](../Model/ProgramPlatformLocale.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **readProgramPlatformLocale**
> \Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale readProgramPlatformLocale($id_program, $id_platform, $id_locale)

Reads a program configuration for a specific platform and locale



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Softonic\NoodleSetupApiSdk\Api\ProgramsPlatformsLocalesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id_program = "id_program_example"; // string | Program identifier
$id_platform = "id_platform_example"; // string | Platform identifier
$id_locale = "id_locale_example"; // string | Locale identifier

try {
    $result = $apiInstance->readProgramPlatformLocale($id_program, $id_platform, $id_locale);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProgramsPlatformsLocalesApi->readProgramPlatformLocale: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id_program** | [**string**](../Model/.md)| Program identifier |
 **id_platform** | **string**| Platform identifier |
 **id_locale** | **string**| Locale identifier |

### Return type

[**\Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale**](../Model/ProgramPlatformLocale.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **replaceProgramPlatformLocale**
> \Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale replaceProgramPlatformLocale($id_program, $id_platform, $id_locale, $body)

Replaces a program configuration for a specific platform and locale

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Softonic\NoodleSetupApiSdk\Api\ProgramsPlatformsLocalesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id_program = "id_program_example"; // string | Program identifier
$id_platform = "id_platform_example"; // string | Platform identifier
$id_locale = "id_locale_example"; // string | Locale identifier
$body = new \Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale(); // \Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale | 

try {
    $result = $apiInstance->replaceProgramPlatformLocale($id_program, $id_platform, $id_locale, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProgramsPlatformsLocalesApi->replaceProgramPlatformLocale: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id_program** | [**string**](../Model/.md)| Program identifier |
 **id_platform** | **string**| Platform identifier |
 **id_locale** | **string**| Locale identifier |
 **body** | [**\Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale**](../Model/ProgramPlatformLocale.md)|  |

### Return type

[**\Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale**](../Model/ProgramPlatformLocale.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateProgramPlatformLocale**
> \Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale updateProgramPlatformLocale($id_program, $id_platform, $id_locale, $body)

Updates a program configuration for a specific platform and locale

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Softonic\NoodleSetupApiSdk\Api\ProgramsPlatformsLocalesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$id_program = "id_program_example"; // string | Program identifier
$id_platform = "id_platform_example"; // string | Platform identifier
$id_locale = "id_locale_example"; // string | Locale identifier
$body = new \Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale(); // \Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale | 

try {
    $result = $apiInstance->updateProgramPlatformLocale($id_program, $id_platform, $id_locale, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProgramsPlatformsLocalesApi->updateProgramPlatformLocale: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id_program** | [**string**](../Model/.md)| Program identifier |
 **id_platform** | **string**| Platform identifier |
 **id_locale** | **string**| Locale identifier |
 **body** | [**\Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale**](../Model/ProgramPlatformLocale.md)|  |

### Return type

[**\Softonic\NoodleSetupApiSdk\Client\Model\ProgramPlatformLocale**](../Model/ProgramPlatformLocale.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

