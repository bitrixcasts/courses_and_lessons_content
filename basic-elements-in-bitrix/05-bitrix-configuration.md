#### Конфигурации старого ядра
Находятся в файле `/bitrix/php_interface/dbconn.php`

#### Конфигурации нового ядра D7
Находятся в файле `/bitrix/.settings.php`

### Получение конфигураций нового ядра

```php
Bitrix\Main\Config\Configuration::getValue('exception_handling');
```

### Дополнительные материалы
1. [Документация: Настройки параметров ядра](https://dev.1c-bitrix.ru/learning/course/index.php?COURSE_ID=43&LESSON_ID=2795&LESSON_PATH=3913.5062.2795)
2. [Документация к классам Bitrix\Main\Config](https://dev.1c-bitrix.ru/api_d7/bitrix/main/config/index.php)


