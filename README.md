# SwaggerClient-php
No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)

This PHP package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 2018-09-12T18:33:43Z
- Build package: io.swagger.codegen.languages.PhpClientCodegen

## Requirements

PHP 5.4.0 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
{
  "repositories": [
    {
      "type": "git",
      "url": "https://github.com/revenuewire/clients-api-sdk-php.git"
    }
  ],
  "require": {
    "revenuewire/clients-api-sdk-php": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/SwaggerClient-php/autoload.php');
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

// Configure API key authorization: api_key
Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');

$api_instance = new Swagger\Client\Api\DefaultApi();
$newClient = new \Swagger\Client\Model\NewClient(); // \Swagger\Client\Model\NewClient | 

try {
    $result = $api_instance->createClient($newClient);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->createClient: ', $e->getMessage(), PHP_EOL;
}

?>
```

## Documentation for API Endpoints

All URIs are relative to *https://client-api.sandbox.revenuewire.io*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*DefaultApi* | [**createClient**](docs/Api/DefaultApi.md#createclient) | **POST** /v1/clients | 
*DefaultApi* | [**getClientById**](docs/Api/DefaultApi.md#getclientbyid) | **GET** /v1/clients/{id} | 
*DefaultApi* | [**getClientByLegacyId**](docs/Api/DefaultApi.md#getclientbylegacyid) | **GET** /v1/clients/legacy/{legacyID} | 
*DefaultApi* | [**updateClientById**](docs/Api/DefaultApi.md#updateclientbyid) | **PUT** /v1/clients/{id} | 


## Documentation For Models

 - [Client](docs/Model/Client.md)
 - [NewClient](docs/Model/NewClient.md)
 - [UpdateClient](docs/Model/UpdateClient.md)


## Documentation For Authorization


## api_key

- **Type**: API key
- **API key parameter name**: x-api-key
- **Location**: HTTP header


## Author




