Imperavi placeholders plugin
=====================

Placeholders plugin for imperavi editor version 10.0

## Introduction

You should try it out if you like:

1. Copy files into plugins folder of editor
2. Activate plugin in editor config
3. Set parameter 'data-placeholders' in editor init config

It's really really easy to get started. Seriously, it's so easy:

``` php
$this->widget(
    'ImperaviRedactorWidget',
    array(
        'options' => array(
            'allowedAttr' =>  array(
                array('span', array('class', 'name', 'contenteditable')),
            )
        ),
        'plugins' => array(
            'placeholders' => array(
                'css' => array('placeholders.css',),
                'js' => array('placeholders.js',),
            )
        ),
        'htmlOptions' => array(
            'data-placeholders' => '[{"name": "placeholder_gallery","value": "Иллюстрации"}]'
        )
    )
);
```
