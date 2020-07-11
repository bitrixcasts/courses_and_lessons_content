Создайте файл в корне проекта, например: `test.php`

Добавьте этот файл в `.gitignore`

Добавьте подключение ядра Bitrix в этот файл и выполните любой код, который хотите протестировать:
```php
<?php
require_once $_SERVER['DOCUMENT_ROOT'] . '/bitrix/modules/main/include/prolog_before.php';

dd(\Bitrix\Main\Config\Configuration::getValue('exception_handling'));
```
