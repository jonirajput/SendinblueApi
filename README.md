Sendinblue API
==============

Clean and simple to use lib for use Sendinblue API.

- [x] tested
- [x] stable
- [x] extensible


> For now the only API available is the SMS api, more is coming later, PRs accepted with love.

Authentication
--------------

```php
<?php

require 'vendor/autoload.php';

use Scoringline\SendinblueApi\Sendinblue;

$sendinblue = new Sendinblue();

$sendinblue->authenticate('ApiKey', ['key' => 'YourPrivateApiKey']);
```


SMS Api usage
-------------

```php
<?php

require 'vendor/autoload.php';

use Scoringline\SendinblueApi\Sendinblue;

$sendinblue = new Sendinblue();

$sendinblue->getSmsApi()->sendSms('+33600000000', 'Your name', 'The message you want to send');
```
