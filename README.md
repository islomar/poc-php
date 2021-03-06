# Playground for learning about PHP and its ecosystem
Playground for PHP ecosystem

## PHP general info
* [PHP-FIG: Framework Interop Group](https://www.php-fig.org/)
 * [PSR: PHP Standard Recommendations](https://www.php-fig.org/psr/)
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

## Style
* PSR:
 * [PSR-1: Basic Coding Standard](https://www.php-fig.org/psr/psr-1/)
 * [PSR-2: Coding Style Guide](https://www.php-fig.org/psr/psr-2/)
 * [PSR-12: Extended Coding Style](https://www.php-fig.org/psr/psr-12/)
* https://pear.php.net/manual/en/standards.php

## CQRS
* http://getprooph.org/

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


## Testing
* Mutation testing: https://github.com/infection/infection
 * [Behat (BDD style)](https://docs.behat.org/en/latest/)
 * Doubles
  * [Mockery](https://github.com/mockery/mockery)


## PHP and Macro-design
* https://medium.com/coding-stones/desarrollando-un-mvp-php-y-clean-architecture-796c55873d9f
* DB migrations: [Phinx](https://book.cakephp.org/phinx/0/en/index.html)

## To be read/studied
* https://www.javier-rodriguez.com/#/blog/Porque%20PHP%20es%20mol%C3%B3n./4
* https://thephp.website/en/issue/php-8-jit/
* Videos:
  * [https://www.youtube.com/watch?v=v2IjMrpZog4](https://www.youtube.com/watch?v=v2IjMrpZog4)
  * https://codely.tv/blog/screencasts/tipos-php-7/
  * [Analizamos el Código en LARAVEL de Brainity 😳 | Auditoría 1](https://www.youtube.com/watch?v=YJqULawVAMQ&t=2s)
  * [CodelyTV: Symfony](https://www.youtube.com/channel/UC9IKtxn9AIGelnYmwYr0Lxw/search?query=symfony)
  * [CodelyTV: PHP](https://www.youtube.com/channel/UC9IKtxn9AIGelnYmwYr0Lxw/search?query=php)
* Versions manager, like SDKMan, virtualenv, rbenv
* Immutability
* Interfaces
* Linters
* Optional
* Enum
* Filter - Map - Reduce
* Lambdas
* Something like ArchUnit for PHP
 * https://github.com/sensiolabs-de/deptrac
* Outside-in TDD with Symfony
* Testing
 * [Behat (BDD style)](https://docs.behat.org/en/latest/)
 * Matchers
 * Doubles
  * [Mockery](https://github.com/mockery/mockery)
