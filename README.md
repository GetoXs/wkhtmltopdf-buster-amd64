wkhtmltopdf-buster-amd64
========================

This repository contains the static compiled binaries from the [wkhtmltopdf project](http://wkhtmltopdf.org/).
More about the functionality of wkhtmltopdf and wkthmltoimage can be found there.

Binaries for __Microsoft Windows__, also installable with composer, can be found here: [github.com/wemersonjanuario/wkhtmltopdf-windows](https://github.com/wemersonjanuario/wkhtmltopdf-windows)

Binaries for __CentOS 7__, also installable with composer, can be found here: [github.com/rvanlaak/wkhtmltopdf-amd64-centos7](https://github.com/rvanlaak/wkhtmltopdf-amd64-centos7)

## Installation

_Hint_:
The version of the binary is equal to the git tag.
To install the latest version, use '0.12.4'.

### Packagist

This package can be found on [Packagist](http://packagist.org) and installed with [Composer](https://getcomposer.org/).

php composer.phar getoxs/wkhtmltopdf-buster-amd64
The binary will then be located at:

vendor/bin/wkhtmltopdf-buster-amd64
### Usage

You can easily use it with [laravel-snappy](https://github.com/barryvdh/laravel-snappy) package by configure `config\snappy.php`

```php
    'pdf' => [
        'enabled' => true,
        'binary'  => env('WKHTML_PDF_BINARY', '../vendor/bin/wkhtmltopdf-amd64'),
    ...
```