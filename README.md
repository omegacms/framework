Omega CMS Framework
===================

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
* A large number of improvements, upgrades, fix and refactors across many components.
* Support for PHP 8.1+.

[Top](#omega-cms-framework)

Install
-------
There are multiple ways you can get Pop PHP Framework into your project.

##### Option 1: Create a New Project

You can create a new project with the `composer create-project` command, which is recommended.

```console
$ composer create-project omegacms/framework project-folder
```

##### Option 2: Clone the Repo

You can clone this repository directly.

```console
$ git clone https://github.com/omegacms/framework.git project-folder
$ cd project-folder
$ composer install
```

##### Option 3: Use `composer require`

You can add it to an existing project with the `composer require` command:

```console
$ composer require omegacms/framework
```

##### Option 4: Use `composer.json`

You can add it your project's `composer.json` file:

    "require": {
        "omegacms/framework": "^1.0.0"
    }


[Top](#omega-cms-framework)

Support
-------

The best way to directly interact with Omega CMS is here on GitHub. You can:

- Contribute code
- Request a feature
- Report an issue

but please do so under the pertinent repository related to the topic at hand. 

[Top](#omega-cms-framework)

