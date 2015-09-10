streams
===============

"tools" is a package of PHP library

Installation
------------
0. Install [Composer](http://getcomposer.org/):

    ```
    curl -sS https://getcomposer.org/installer | php
    ```

0. Add the streams dependency:

    ```
    php composer.phar require 'pulyavin/tools:0.*' 
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

