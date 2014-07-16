yii2-popover-x
=================

An extended popover widget for Yii Framework 2 based on the [bootstrap-popover-x jQuery plugin](http://plugins.krajee.com/popover-x) by Krajee. This plugin
is an extended popover JQuery plugin which combines both the popover and bootstrap modal features and includes various new styling enhancements. This widget
can be setup just like the builtin `yii\bootstrap\Modal`, with some additional enhancements.

> NOTE: This extension depends on the [kartik-v/yii2-widgets](https://github.com/kartik-v/yii2-widgets) extension which in turn depends on the 
[yiisoft/yii2-bootstrap](https://github.com/yiisoft/yii2/tree/master/extensions/bootstrap) extension. Check the 
[composer.json](https://github.com/kartik-v/yii2-popover-x/blob/master/composer.json) for this extension's requirements and dependencies. 
Note: Yii 2 framework is still in active development, and until a fully stable Yii2 release, your core yii2-bootstrap packages (and its dependencies) 
may be updated when you install or update this extension. You may need to lock your composer package versions for your specific app, and test 
for extension break if you do not wish to auto update dependencies.

### Demo
You can see detailed [documentation and examples](http://demos.krajee.com/popover-x) on usage of the extension.

## Installation

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

> Note: You must set the `minimum-stability` to `dev` in the **composer.json** file in your application root folder before installation of this extension.

Either run

```
$ php composer.phar require kartik-v/yii2-popover-x "dev-master"
```

or add

```
"kartik-v/yii2-popover-x": "dev-master"
```

to the ```require``` section of your `composer.json` file.

## Usage

### PopoverX

```php
use kartik\popover\PopoverX;

PopoverX::begin([
    'header' => 'Hello world',
    'footer' => Html::button('View', ['class'=>'btn btn-primary']),
    'toggleButton' => ['label' => 'Open Popover'],
]);

echo '<p class="text-justify">' .
    'Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor.' . 
    '</p>';

PopoverX::end();
```

## License

**yii2-popover-x** is released under the BSD 3-Clause License. See the bundled `LICENSE.md` for details.