
<p align="center"><img src="/art/socialcard.png" alt="Social Card of Laravel Activity Log"></p>

[![Latest Stable Version](https://poser.pugx.org/creative-support-system/coding-style/v)](//packagist.org/packages/creative-support-system/coding-style)
[![Total Downloads](https://poser.pugx.org/creative-support-system/coding-style/downloads)](//packagist.org/packages/creative-support-system/coding-style)
[![Coverage Status](https://coveralls.io/repos/github/Creative-Support-System/coding-style/badge.svg?branch=main)](https://coveralls.io/github/Creative-Support-System/coding-style?branch=main)
[![License](https://poser.pugx.org/creative-support-system/coding-style/license)](//packagist.org/packages/creative-support-system/coding-style)

# CodeIgniter Coding Style

This repository contains the coding style followed by Worksome.

It includes configuration for `php-cs-fixer`, `psalm`, `phpstan` and `rector`.

## Setup
Install this composer package

```
composer require creative-support-system/coding-style --dev
```

Run the generate command for generating the config files.
```
composer generate-coding-style-stubs
```

Add the following section to your `composer.json` file
```json
"scripts": {
    "phpcs": "vendor/bin/phpcs",
    "php-cs-fixer": "vendor/bin/php-cs-fixer fix --ansi",
    "php-cs-fixer-ci": "vendor/bin/php-cs-fixer fix --dry-run --ansi",
    "phpstan": "vendor/bin/phpstan analyse",
    "rector-ci": "vendor/bin/rector process --dry-run --ansi",
    "rector": "vendor/bin/rector process --ansi"
},
```

## Usage

For using it simply run one of the scripts added to composer.
```
$ composer php-cs-fixer
$ composer phpstan
$ composer rector-ci
```

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
