# Getting started with PHP

The PHP SDK for Fireblocks API

[![Current version](https://img.shields.io/packagist/v/d-andreevich/fireblocks-sdk-php.svg?logo=composer)](https://packagist.org/packages/d-andreevich/fireblocks-sdk-php)
[![Monthly Downloads](https://img.shields.io/packagist/dm/d-andreevich/fireblocks-sdk-php.svg)](https://packagist.org/packages/d-andreevich/fireblocks-sdk-php/stats)
[![Total Downloads](https://img.shields.io/packagist/dt/d-andreevich/fireblocks-sdk-php.svg)](https://packagist.org/packages/d-andreevich/fireblocks-sdk-php/stats)

## Basics
This repository contains the PHP SDK for Fireblocks API.
For the complete API reference, go to the [API reference](https://docs.fireblocks.com/api).


### Requirements
`PHP >=7.2.`

`GuzzleHttp >=6.0.X`

## Installation

You can install the Provider as a composer package.

```bash
composer require d-andreevich/fireblocks-sdk-php
```

## Usage
### Before You Begin
Make sure you have the credentials for Fireblocks API Services. Otherwise, please contact Fireblocks support for further instructions on how to obtain your API credentials.

### Start
Once you have retrieved a component, please refer to the [documentation of the Fireblocks](https://docs.fireblocks.com/api/?python#introduction)
for further information on how to use it.


```php
<?php

use FireblocksSdkPhp\FireblocksSDK;

$private_key = file_get_contents('fireblocks_secret.key');
$api_key = 'XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX';
$fireblocks = new FireblocksSDK($private_key, $api_key);
$result = $fireblocks->get_gas_station_info();
```

You can use the Python examples from the [documentation of the Fireblocks](https://docs.fireblocks.com/api/?python#introduction), all methods have the same names, all functionality is duplicated from [fireblocks-sdk-py](https://github.com/fireblocks/fireblocks-sdk-py).