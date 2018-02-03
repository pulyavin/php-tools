streams
===============

"tools" is a package of PHP library

Installation
------------
0. Install [Composer](http://getcomposer.org/):

    ```
    curl -sS https://getcomposer.org/installer | php
    ```

1. Add dependency

```
{
    "require": {
        "pulyavin/tools": "dev-master"
    },
    "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/pulyavin/miner"
        }
    ]
}
```

2. Update:

```
php composer.phar update
```

Usage
-----

So you can get a random user agent, like this

```php
use pulyavin\tools\UserAgents;

$agent = new UserAgents;

// get random user agent
var_dump($agent->getRand());

// get random user agent of list
var_dump($agent->getRand(['FFWin', 'FFMac', 'FFLin']));
```

