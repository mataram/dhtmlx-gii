yii2-dhtmlx-gii-generators
=====================

This generator generates the grid on a given url with the help of DHTMLX Grid.

## Installation

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
$ php composer.phar require "dhtmlx/dhtmlx-gii": "dev-master"
```

or add

```
"dhtmlx/dhtmlx-gii": "dev-master"
```

to the ```require``` section of your `composer.json` file.

## Usage

```php
//if your gii modules configuration looks like below:
    $config['bootstrap'][] = 'gii';
    $config['modules']['gii'] = 'yii\gii\Module';

//remove this two lines
```

```php
//Add this into common/config/main-local.php
    'bootstrap' => 'gii',
    'modules' => [
        'gii' => [
            'class' => 'yii\gii\Module',
            'generators' => [
                'doubleModel' => [
                    'class' => 'dhtmlx\generators\Generator',
                ],
            ],
        ],
    ],
```