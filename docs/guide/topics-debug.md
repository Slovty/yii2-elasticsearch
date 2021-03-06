Using the Elasticsearch DebugPanel
----------------------------------

The yii2 Elasticsearch extension provides a `DebugPanel` that can be integrated with the
yii debug module and shows the executed Elasticsearch queries. It also allows to run
these queries and view the results.

Add the following to you application config to enable it (if you already have the debug module
enabled, it is sufficient to just add the panels configuration):

```php
    // ...
    'bootstrap' => ['debug'],
    'modules' => [
        'debug' => [
            'class' => 'yii\\debug\\Module',
            'panels' => [
                'elasticsearch' => [
                    'class' => 'yii\\elasticsearch\\DebugPanel',
                ],
            ],
        ],
    ],
    // ...
```

![Elasticsearch DebugPanel](images/debug.png)
