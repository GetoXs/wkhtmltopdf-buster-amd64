wkhtmltopdf-buster-amd64
========================

This repository contains the static compiled binaries from the [wkhtmltopdf project](http://wkhtmltopdf.org/).
More about the functionality of wkhtmltopdf and wkthmltoimage can be found there.

## Installation

_Hint_:
The version of the binary is equal to the git tag.

### Packagist

This package can be found on [Packagist](https://packagist.org/packages/getoxs/wkhtmltopdf-buster-amd64) and installed with [Composer](https://getcomposer.org/).

```
php composer.phar getoxs/wkhtmltopdf-buster-amd64
```

The binary will then be located at: `vendor/bin/wkhtmltopdf-buster-amd64`
### Usage

You can easily use it with [laravel-snappy](https://github.com/barryvdh/laravel-snappy) package by configure `config\snappy.php`

```php
    'pdf' => [
        'enabled' => true,
        'binary'  => env('WKHTML_PDF_BINARY', '../vendor/bin/wkhtmltopdf-amd64'),
    ...
```