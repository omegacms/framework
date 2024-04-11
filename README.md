OmegaCMS Framework
=================

* [Overview](#overview)
* [New Features](#new-features)
* [Install](#install)
* [Support](#support)

Release Information
-------------------
Omega Framework 1.0.0

Overview
--------
This repository contains the `composer.json` file to install the full stack of OmegaCMS Framework.
All the components listed below will be installed:

|                                                        | Components                                           |                                                                         |
|--------------------------------------------------------|------------------------------------------------------|-------------------------------------------------------------------------|
| [application](https://github.com/omegacms/application) | [filesystem](https://github.com/omegacms/filesystem) | [serializable-closure](https://github.com/omegacms/serializable-closure)|
| [cache](https://github.com/omegacms/cache)             | [helpers](https://github.com/omegacms/helpers)       | [session](https://github.com/omegacms/session)                          |
| [config](https://github.com/omegacms/config)           | [http](https://github.com/omegacms/http)             | [support](https://github.com/omegacms/support)                          |
| [container](https://github.com/omegacms/container)     | [logging](https://github.com/omegacms/logging)       | [testing](https://github.com/omegacms/testing)                          |
| [database](https://github.com/omegacms/database)       | [model](https://github.com/omegacms/model)           | [validation](https://github.com/omegacms/validating)                    |
| [email](https://github.com/omegacms/email)             | [queue](https://github.com/omegacms/queue)           | [view](https://github.com/omegacms/view)                                |
| [environment](https://github.com/omegacms/environment) | [renderer](https://github.com/omegacms/renderer)     |                                                                         |
| [exceptions](https://github.com/omegacms/exceptions)   | [routing](https://github.com/omegacms/routing)       |                                                                         |

New Features
------------
* A large number of improvements, upgrades and refactors across many components.
* Support for PHP 8.1+.
* Support for PHP <=7.4 has been deprecated.
* PHPUnit tests refactored for PHPUnit 10.0+.
* Reference the [CHANGELOG.md](https://github.com/popphp/popphp-framework/blob/master/CHANGELOG.md) for further details.

[Top](#pop-php-framework)

Install
-------
There are multiple ways you can get Pop PHP Framework into your project.

##### Option 1: Create a New Project

You can create a new project with the `composer create-project` command, which is recommended.
This way, you will have access to the CLI-helper script `kettle` in the main project folder:

```console
$ composer create-project popphp/popphp-framework project-folder
```

##### Option 2: Clone the Repo

You can clone this repository directly, which will also install the `kettle` script
in the main project folder:

```console
$ git clone https://github.com/popphp/popphp-framework.git popphp
$ cd popphp
$ composer install
```

##### Option 3: Use `composer require`

You can add it to an existing project with the `composer require` command:

```console
$ composer require popphp/popphp-framework
```

##### Option 4: Use `composer.json`

You can add it your project's `composer.json` file:

    "require": {
        "popphp/popphp-framework": "^5.3.0"
    }


[Top](#pop-php-framework)

Kettle
------

### CLI Helper

`pop-kettle`

If choose to install the framework in a way that the `pop-kettle` CLI-helper script is not available
in the main project folder (options 3 and 4), you can place a copy of the script from the
`vendor/popphp/pop-kettle/kettle` location in the main project folder (adjacent to the `vendor` folder):

```bash
$ cp vendor/popphp/pop-kettle/kettle .
$ cp vendor/popphp/pop-kettle/kettle.inc.php .
```
Once you've copied the scripts over, you have to change the reference to the script's
config file from:

```php
    $app = new Pop\Application(
        $autoloader, include __DIR__ . '/config/app.console.php'
    );
```

to

```php
    $app = new Pop\Application(
        $autoloader, include __DIR__ . '/vendor/popphp/pop-kettle/config/app.console.php'
    );
```

and make sure the newly copied `kettle` script is set to execute (755)

```bash
$ chmod 755 kettle
```

[Top](#pop-php-framework)

Support
-------

The best way to directly interact with Pop PHP is here on GitHub. You can:

- Contribute code
- Request a feature
- Report an issue

but please do so under the pertinent repository related to the topic at hand. 

Besides interacting with the various repositories here on GitHub, there are
a few other ways to participate in the Pop PHP community:

- [Slack](https://popphp.slack.com)
- [Discord](https://discord.gg/TZjgT74U7E)
- [X](https://x.com/popphpframework)


[Top](#pop-php-framework)

