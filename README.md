PHPUnit-Printer
===

A PhpUnit result printer.
This is a fork of `kujira/phpunit-printer` modified to be used with the symfony framework.

## Requirements

 * A symfony installation, tested with 4.2.28
 * PHP 5.3.0 or later
 * the symfony/phpunit-bridge `composer require --dev symfony/phpunit-bridge`

## How it looks

![Alt text](/kujira-phpunit-result-printer.jpg?raw=true "Kujira phpunit result printer")

## Installation

This package has been modified to work when used relatively and in dev-requirements like 

`composer require --dev "g33z/phpunit-printer"`

---

* Add to your phpunit.xml

```xml
   <phpunit
        bootstrap="config/bootstrap.php"
        colors="true"
        printerFile="vendor/kujira/phpunit-printer/src/Printer.php"
        printerClass="Kujira\PHPUnit\Printer"
   >
```

* Configure your php.ini default_charset to UTF-8

* Configure your terminal to display UTF-8 charset and use a UTF-8 compatible font like DejaVu Sans Mono

## License

The PHPUnit-Printer is licensed under the [MIT license](LICENSE).