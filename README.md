# poc-php
Playground for PHP ecosystem

## PHP general info
* It's installed on /etc/php/7.1
* You can change the running version using `update-alternatives --set php /usr/bin/phpX.Y`
* `php --ini`
  * Find your php.ini file
* `php -m`
  * See your modules
* Code coverage
  * You need XDebug.
    * You can check it with `php --ri xdebug`
    * Check if the module appears with `php -m`
    * http://www.dieuwe.com/blog/xdebug-ubuntu-1604-php7
  * You must configure a whitelist: https://phpunit.de/manual/current/en/code-coverage-analysis.html#code-coverage-analysis.whitelisting-files
  * https://phpunit.de/manual/current/en/code-coverage-analysis.html


## Steps for creating a Laravel 5.5 project
* Prerequisites:
    * PHP 7.1
* `sudo apt-get install php7.1-zip`
* `sudo apt-get install php7.1-mbstring`
* `composer global require "laravel/installer"`
* `composer create-project --prefer-dist laravel/laravel blog "5.5.*"`
* Install dependencies: `composer install`
* Run the tests:
    * `./vendor/bin/phpunit`
    * Other options:
        1. `wget http://getcomposer.org/composer.phar`
        2. `php composer.phar install`
        3. `php bin/phpunit`
        4. `php bin/phpunit --coverage-text`
        5. `php bin/phpunit --coverage-html report/`
        6. `open report/index.html`
* Run the server: `php artisan serve`


## Interesting links
* **PHP**
    * https://packagist.org/: Packagist is the main Composer repository. It aggregates public PHP packages installable with Composer.
    * https://www.airpair.com/php/posts/best-practices-for-modern-php-development
    * Composer:
        * https://blog.bugsnag.com/best-practices-using-composer/
        * https://www.sitepoint.com/composer-global-require-considered-harmful/
        * https://www.digitalocean.com/community/tutorials/how-to-install-and-use-composer-on-ubuntu-14-04
        * https://getcomposer.org/doc/articles/versions.md
    * Testing:
        * PHPUnit
        * Mockery
        * Prophecy
* **Static analysis tools**
 * https://github.com/phpstan/phpstan
 * https://github.com/phan/phan
* **Refactoring legacy code**
 * https://github.com/rectorphp/rector
* **Laravel**
    * https://getcomposer.org/doc/faqs/should-i-commit-the-dependencies-in-my-vendor-directory.md
    * http://www.laravelbestpractices.com/
    * https://forge.laravel.com/
    * Homestead: Vagran with Laravel for local development

