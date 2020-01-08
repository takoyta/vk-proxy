# vk-php-sdk with proxy


## 1. Prerequisites

* PHP 7.1 or later

## 2. Installation

add to composer.json:

```json
    "repositories":
    [
      {
        "type": "vcs",
        "url": "https://github.com/takoyta/vk-proxy"
      }
    ],
    ...
    "require": {
      "takoyta/vk-proxy": "dev-master"
```

## 3. Initialization

Create VKApiClient object using the following code:

```php
$vk = new VK\Client\VKApiClient();
$vk->setProxy('127.0.0.1:8080', CURLPROXY_HTTP);
```

