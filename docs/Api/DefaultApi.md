# Swagger\Client\DefaultApi

All URIs are relative to *https://client-api.sandbox.revenuewire.io*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createClient**](DefaultApi.md#createClient) | **POST** /v1/clients | 
[**getClientById**](DefaultApi.md#getClientById) | **GET** /v1/clients/{id} | 
[**updateClientById**](DefaultApi.md#updateClientById) | **PUT** /v1/clients/{id} | 


# **createClient**
> \Swagger\Client\Model\Client createClient($newClient)



### Example
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

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **newClient** | [**\Swagger\Client\Model\NewClient**](../Model/\Swagger\Client\Model\NewClient.md)|  |

### Return type

[**\Swagger\Client\Model\Client**](../Model/Client.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getClientById**
> \Swagger\Client\Model\Client getClientById($id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');

$api_instance = new Swagger\Client\Api\DefaultApi();
$id = "id_example"; // string | 

try {
    $result = $api_instance->getClientById($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->getClientById: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |

### Return type

[**\Swagger\Client\Model\Client**](../Model/Client.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateClientById**
> \Swagger\Client\Model\Client updateClientById($id, $updateClient)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('x-api-key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('x-api-key', 'Bearer');

$api_instance = new Swagger\Client\Api\DefaultApi();
$id = "id_example"; // string | 
$updateClient = new \Swagger\Client\Model\UpdateClient(); // \Swagger\Client\Model\UpdateClient | 

try {
    $result = $api_instance->updateClientById($id, $updateClient);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->updateClientById: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |
 **updateClient** | [**\Swagger\Client\Model\UpdateClient**](../Model/\Swagger\Client\Model\UpdateClient.md)|  |

### Return type

[**\Swagger\Client\Model\Client**](../Model/Client.md)

### Authorization

[api_key](../../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

