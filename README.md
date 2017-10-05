# Yii2 Cookie Consent

[![Latest Stable Version](https://poser.pugx.org/hiqdev/yii2-cookie-consent/v/stable)](https://packagist.org/packages/hiqdev/yii2-cookie-consent)
[![Total Downloads](https://poser.pugx.org/hiqdev/yii2-cookie-consent/downloads)](https://packagist.org/packages/hiqdev/yii2-cookie-consent)
[![Build Status](https://img.shields.io/travis/hiqdev/yii2-cookie-consent.svg)](https://travis-ci.org/hiqdev/yii2-cookie-consent)
[![Scrutinizer Code Coverage](https://img.shields.io/scrutinizer/coverage/g/hiqdev/yii2-cookie-consent.svg)](https://scrutinizer-ci.com/g/hiqdev/yii2-cookie-consent/)
[![Scrutinizer Code Quality](https://img.shields.io/scrutinizer/g/hiqdev/yii2-cookie-consent.svg)](https://scrutinizer-ci.com/g/hiqdev/yii2-cookie-consent/)

Provides really easy alerting users about the use of
cookies on your site.

Cookie consent is required to comply with the [EU Cookie Law].

Additionally it detects if cookie is disabled in user's browser
and redirects user to predefined page.

Works by adding Behavior to the Application View.
Behavior listens to [EVENT_END_BODY] and echos the consent script.

[EVENT_END_BODY]:   http://www.yiiframework.com/doc-2.0/yii-web-view.html#EVENT_END_BODY-detail
[EU Cookie Law]:    http://ec.europa.eu/ipg/basics/legal/cookies/index_en.htm

## Installation

The preferred way to install this yii2-extension is through [composer](http://getcomposer.org/download/).

Either run

```sh
php composer.phar require "hiqdev/yii2-cookie-consent"
```

or add

```json
"hiqdev/yii2-cookie-consent": "*"
```

to the require section of your composer.json.

## Configuration

This extension is supposed to be used with [composer-config-plugin].

Else look [src/config/web.php] for cofiguration example.

Available configuration parameters:

- `cookieConsent.disabled`
- `cookieConsent.params`
    - `message` - message to be shown
    - `dismiss`
    - `theme`
    - `more`
    - `moreLink`
    - `failUrl` - url user will be redirected when cookies are disabled

For more details please see [src/config/params.php].

[composer-config-plugin]:   https://github.com/hiqdev/composer-config-plugin
[src/config/web.php]:       src/config/web.php
[src/config/params.php]:    src/config/params.php

## License

This project is released under the terms of the BSD-3-Clause [license](LICENSE).
Read more [here](http://choosealicense.com/licenses/bsd-3-clause).

Copyright © 2017, HiQDev (http://hiqdev.com/)

## Acknowledgements

- https://github.com/insites/cookieconsent
- https://github.com/cinghie/yii2-cookie-consent
