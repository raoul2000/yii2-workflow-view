THIS RELEASE IS A DRAFT SO PLEASE DO NOT USE YET.

# yii2-workflow-view

[![License](https://poser.pugx.org/raoul2000/yii2-workflow/license)](https://packagist.org/packages/raoul2000/yii2-workflow-view)

*A Widget to display your workflow*

## Installation

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist raoul2000/yii2-workflow-view "*"
```

or add

```
"raoul2000/yii2-workflow-view": "*"
```

to the require section of your `composer.json` file.

**Note that this widget requires yii2-workflow**

## Usage

To display a workflow with the widget, you must have ... a workflow to display ! Once you have
it, just assign it to the `workflow` parameter.

In the example below we are assuming that the `Post` model is attached to a *SimpleWorkflowBehavior* and correctly
initialized.

```php
<?php
$post = new app\models\Post();

raoul2000\workflow\view\WorkflowViewWidget::widget([
	'workflow'    => $post,
	'containerId' => 'myWorkflowView'
]);
?>

<div id="myWorkflowView" style="height: 400px;"></div>
```

For more information on the *SimpleWorkflowBehavior*, please refer to [yii2-workflow](https://github.com/raoul2000/yii2-workflow)
License
-------

**yii2-workflow-view** is released under the BSD 3-Clause License. See the bundled `LICENSE.md` for details.

[![Yii2](https://img.shields.io/badge/Powered_by-Yii_Framework-green.svg?style=flat)](http://www.yiiframework.com/)


