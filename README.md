Sylius-Sandbox [![Build status...](https://secure.travis-ci.org/Sylius/Sylius-Sandbox.png)](http://travis-ci.org/Sylius/Sylius-Sandbox)
==============

Sylius is **developer friendly** e-commerce framework built on top of [Symfony2](http://symfony.com).  
We also plan to provide a rich featured end-user application in future.

This is sandbox application which shows some examples of the Sylius bundles usage.  
It's also testing ground for new features planned for [main Sylius application](http://github.com/Sylius/Sylius).

This repository **will never** be stable.

[DEMO](http://sylius.org/sandbox).

Quick installation
------------------

Clone this repository with this command.

``` bash
$ git clone http://github.com/Sylius/Sylius-Sandbox.git
```

Open `sandbox/config/container/parameters.yml.dist`, set your values and save as `parameters.yml`.

Install dependencies using composer.

``` bash
$ wget http://getcomposer.org/composer.phar
$ php composer.phar install --prefer-dist
```

Create database schema and dump assetic assets by typing following commands inside console.

``` bash
$ ./bin/rebuild-database
$ php sandbox/console assetic:dump
```

Open up ``/path/to/Sylius-Sandbox/public/dev.php`` in your browser and play with the application.

[Behat](http://behat.org) scenarios
-----------------------------------

``` bash
$ ./bin/behat @SyliusSandboxBundle
```

[phpspec2](http://phpspec.net) examples
---------------------------------------

``` bash
$ bin/phpspec run -f pretty
```

Contributing
------------

All informations about contributing to Sylius can be found on [this page](http://sylius.readthedocs.org/en/latest/contributing/index.html).

Mailing lists
-------------

### Users.

If you are using this application and have any questions, feel free to ask on users mailing list.
[Mail](mailto:sylius@googlegroups.com) or [view it](http://groups.google.com/group/sylius).

### Developers.

If you want to contribute, and develop this application, use the developers mailing list.
[Mail](mailto:sylius-dev@googlegroups.com) or [view it](http://groups.google.com/group/sylius-dev).

Sylius twitter account
----------------------

If you want to keep up with updates, [follow the official Sylius account on twitter](http://twitter.com/_Sylius)
or [follow me](http://twitter.com/pjedrzejewski).

Bug tracking
------------

This application uses [GitHub issues](https://github.com/Sylius/Sylius-Sandbox/issues).
If you have found bug, please create an issue.

MIT License
-----------

License can be found [here](https://github.com/Sylius/Sylius-Sandbox/blob/master/LICENSE).

Authors
-------

The application was originally created by [Paweł Jędrzejewski](http://pjedrzejewski.com).
See the list of [contributors](https://github.com/Sylius/Sylius-Sandbox/contributors).
