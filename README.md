# NoodleSetupApiSdk
API that allows configure programs for Noodle

This PHP package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 1.0.0
- Package version: 1.0.0
- Build package: io.swagger.codegen.languages.PhpClientCodegen
For more information, please visit [http://corporate.softonic.com/contact-us](http://corporate.softonic.com/contact-us)

## Requirements

PHP 5.5 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
{
  "repositories": [
    {
      "type": "git",
      "url": "https://github.com/softonic/sdk_noodle-setup-api.git"
    }
  ],
  "require": {
    "softonic/sdk_noodle-setup-api": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/NoodleSetupApiSdk/vendor/autoload.php');
```

## Tests

To run the unit tests:

```
composer install
./vendor/bin/phpunit
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

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

## Documentation for API Endpoints

All URIs are relative to *https://noodle-setup-v1.sftapi.com*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ProgramLocaleConfigurationApi* | [**programsIdProgramLocalesGet**](docs/Api/ProgramLocaleConfigurationApi.md#programsidprogramlocalesget) | **GET** /programs/{id_program}/locales | Finds configurations for program in all Softonic locales
*ProgramLocaleConfigurationApi* | [**programsIdProgramLocalesIdLocaleDelete**](docs/Api/ProgramLocaleConfigurationApi.md#programsidprogramlocalesidlocaledelete) | **DELETE** /programs/{id_program}/locales/{id_locale} | Deletes a program configuration for a specific locale
*ProgramLocaleConfigurationApi* | [**programsIdProgramLocalesIdLocaleGet**](docs/Api/ProgramLocaleConfigurationApi.md#programsidprogramlocalesidlocaleget) | **GET** /programs/{id_program}/locales/{id_locale} | Finds configurations for program and Softonic locale
*ProgramLocaleConfigurationApi* | [**programsIdProgramLocalesIdLocalePatch**](docs/Api/ProgramLocaleConfigurationApi.md#programsidprogramlocalesidlocalepatch) | **PATCH** /programs/{id_program}/locales/{id_locale} | Updates a program configuration for a specific locale
*ProgramLocaleConfigurationApi* | [**programsIdProgramLocalesIdLocalePut**](docs/Api/ProgramLocaleConfigurationApi.md#programsidprogramlocalesidlocaleput) | **PUT** /programs/{id_program}/locales/{id_locale} | Replaces a program configuration for a specific locale
*ProgramLocaleConfigurationApi* | [**programsIdProgramLocalesPost**](docs/Api/ProgramLocaleConfigurationApi.md#programsidprogramlocalespost) | **POST** /programs/{id_program}/locales | Creates a program configuration for a specific locale


## Documentation For Models

 - [Program](docs/Model/Program.md)


## Documentation For Authorization


## noodle_setup

- **Type**: OAuth
- **Flow**: application
- **Authorization URL**: 
- **Scopes**: 
 - **noodle_setup.find.program.locales**: Find Program configurations for all Softonic locales
 - **noodle_setup.read.program.locales**: Read Program configuration for a Softonic locale
 - **noodle_setup.create.program.locales**: Create Program configuration for a Softonic locale
 - **noodle_setup.replace.program.locales**: Replace Program configuration for a Softonic locale
 - **noodle_setup.update.program.locales**: Update Program configuration for a Softonic locale
 - **noodle_setup.delete.program.locales**: Delete Program configuration for a Softonic locale


## Author

development@softonic.com


