<div align="center">
  <img src="https://github.com/user-attachments/assets/b268ae9e-7c8a-4ade-95da-b4ac6fce6eea"/>
</div>
<div align="center">

# Treblle

<a href="https://docs.treblle.com/en/integrations" target="_blank">Integrations</a>
<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
<a href="http://treblle.com/" target="_blank">Website</a>
<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
<a href="https://docs.treblle.com" target="_blank">Docs</a>
<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
<a href="https://blog.treblle.com" target="_blank">Blog</a>
<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
<a href="https://twitter.com/treblleapi" target="_blank">Twitter</a>
<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
<a href="https://treblle.com/chat" target="_blank">Discord</a>
<br />

  <hr />
</div>

API Intelligence Platform. 🚀

Treblle is a lightweight SDK that helps Engineering and Product teams build, ship & maintain REST-based APIs faster.

## Features

<div align="center">
  <br />
  <img src="https://github.com/user-attachments/assets/02afd9f5-ab47-48ff-929a-0f3fcddcca34"/>
  <br />
  <br />
</div>

- [API Monitoring & Observability](https://www.treblle.com/features/api-monitoring-observability)
- [Auto-generated API Docs](https://www.treblle.com/features/auto-generated-api-docs)
- [API analytics](https://www.treblle.com/features/api-analytics)
- [Treblle API Score](https://www.treblle.com/features/api-quality-score)
- [API Lifecycle Collaboration](https://www.treblle.com/features/api-lifecycle)
- [Native Treblle Apps](https://www.treblle.com/features/native-apps)



## Treblle API Tools (Laravel)

[![Latest Version](https://img.shields.io/packagist/v/treblle/treblle-api-tools-laravel)](https://packagist.org/packages/treblle/treblle-api-tools-laravel)
[![PHP Version](https://img.shields.io/packagist/php-v/treblle/treblle-api-tools-laravel.svg?style=flat-square)](https://php.net)
[![Tests](https://github.com/treblle/treblle-api-tools-laravel/actions/workflows/tests.yml/badge.svg)](https://github.com/treblle/treblle-api-tools-laravel/actions/workflows/tests.yml)
[![Total Downloads](https://img.shields.io/packagist/dt/treblle/treblle-api-tools-laravel)](https://packagist.org/packages/treblle/treblle-api-tools-laravel)
[![MIT Licence](https://img.shields.io/packagist/l/treblle/treblle-api-tools-laravel)](LICENSE)

Treblle makes it super easy to understand what’s going on with your APIs and the apps that use them. Just by adding
Treblle to your API out of the box you get:

* Real-time API monitoring and logging
* Auto-generated API docs with OAS support
* API analytics
* Quality scoring
* One-click testing
* API management on the go
* Supports Laravel Vapor and Laravel Octane
* and more...


A set of useful tools for building APIs in Laravel.

## Requirements

* PHP 8.2+
* Laravel 10+

## Installation

```bash
composer require treblle/treblle-api-tools-laravel
```

## Usage

### Headers

#### Authorization

You can use the Authorization Header can be used like the following:

```php
use Treblle\Tools\Http\Enums\Headers\AuthScheme;
use Treblle\Tools\Http\Headers\Authorization;

$auth = new Authorization(
    type: AuthScheme::BEARER,
    credentials: 'YOUR_API_TOKEN_HERE',
);

// Turn the header into an array
$array = $auth->toArray();
//[
//    'type' => AuthScheme::BEARER,
//    'credentials' => 'YOUR_API_TOKEN_HERE'
//]

// Turn the header into a header
$header = $auth->toHeader();
//[
//    'Authorization' => 'Bearer YOUR_API_TOKEN_HERE',
//]
```

## Support

If you have problems of any kind feel free to reach out via <https://treblle.com> or email hello@treblle.com, and we'll
do our best to help you out.

## License

Copyright 2022., Treblle Limited. Licensed under the MIT license:
http://www.opensource.org/licenses/mit-license.php
