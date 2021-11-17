# PHP Library for the Lazada Open API
Usage of this library is also available at [Lazada Open API](https://open.lazada.com)

Requirements
-----

Version 0.1

Requirements
-----

PHP SDK requires PHP 5 or newer version

Composer Installation
-----

Run the following command:
```bash
composer require trungnt309193/lazop-sdk-php
```

Usage
-----

Sample usage:
```php
use trungnt309193\PHPLazadaSDK\LazopClient;
use trungnt309193\PHPLazadaSDK\LazopRequest;

...
$c = new LazopClient('https://api.lazada.test/rest', '${appKey}', '${appSecret}');
$request = new LazopRequest('/mock/api/get');
$request->addApiParam('api_id',1);
$request->addHttpHeaderParam('cx','test');
    
var_dump($c->execute($request));
...

```
