# AlphaID

## Install

```bash
composer require youcloud/alphaid
```

## Usage

```php
use YogCloud\AlphaID;

$id = new AlphaID();
$code = $id->encode(PHP_INT_MAX);
var_dump($code, $id->decode($code));

$code = $id->encode(PHP_INT_MAX, PHP_VERSION_ID);
var_dump($code, $id->decode($code));

$code = $id->encode([PHP_INT_MAX, PHP_VERSION_ID]);
var_dump($code, $id->decode($code));
```
