simgroep/coding-standards
===========================

Coding standard configuration for SIMGroep PHP projects using `fabpot/php-cs-fixer`

## Installation

```
$ composer require simgroep/coding-standards
```

## Examples

Only check for coding standard violations:

```
$ ./vendor/bin/php-cs-fixer fix --dry-run --diff --config=vendor/simgroep/coding-standard/.php_cs.dist --stop-on-violation --allow-risky=yes
```

Fix coding standard violations:

```
$ ./vendor/bin/php-cs-fixer fix --diff --config=vendor/simgroep/coding-standard/.php_cs.dist --stop-on-violation --allow-risky=yes
```

## PhpStorm integration

Start by installing this library global:

```
$ composer global require simgroep/coding-standards
```

Open PhpStorm and navigate to "settings" -> "tools" -> add one (+).
Disable "Immediate fily synchronization".

Program: `/Users/<username>/.composer/vendor/bin/php-cs-fixer`

Arguments: `fix $FileDir$/$FileName$ --config-file=/Users/<username>/.composer/vendor/simgroep/coding-standard/.php_cs`

Working dir: `$ProjectFileDir$`
