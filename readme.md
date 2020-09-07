## About
PhpCsFixer's fixer to convert single quotes to double quotes for simple strings.

## Installation
Install package:
`composer require krzysztofrewak/php-cs-double-quote-fixer --dev`

Add in `ecs.php` configuration file:
```php
return static function (ContainerConfigurator $containerConfigurator): void {
    $services = $containerConfigurator->services();
    $service = $services->set(\KrzysztofRewak\PhpCsFixer\DoubleQuoteFixer\DoubleQuoteFixer::class);
};
```

### Thanks
Thanks for Marcel Pociot for his DoubleQuoteFixer: https://github.com/mpociot/PHP-CS-Fixer/blob/master/Symfony/CS/Fixer/Contrib/DoubleQuoteFixer.php