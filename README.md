# ZF1-Psysh

This is a very simple integration between [psysh](https://github.com/bobthecow/psysh) and [ZF1](https://github.com/zendframework/zf1)

## Installation
```
composer require giorgiolucca/zf1-psysh
```

## Example

Type command
```
$ vendor/bin/zf1-psysh
```
And enjoy!
```
>>> ls # To list scope variables ($bootstrap, $config, $registry)
>>> $doctrine = $bootstrap->bootstrap('doctrine')->getResource('doctrine') # If you integrate your application with Doctrine ORM (like one resource)
>>> $registryCache = $registry->get('cache'); # If you register one dependency with this name
```