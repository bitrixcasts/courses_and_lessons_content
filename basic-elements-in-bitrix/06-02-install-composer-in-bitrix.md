### Подключение composer
Скачайте и установите [Composer](https://getcomposer.org/download/), если он еще не установлен у вас.

#### Установка зависимостей
Создайте файл `/local/php_interface/composer.json` со следующим содержимым:
```json
{
}
```

Выполните команду внутри директории `/local/php_interface/`
```shell script
composer require symfony/var-dumper
```

Исключите директорию `vendor` из отслеживания git, добавьте следующий код в файл `.gitignore`
```text
local/php_interface/vendor
```

#### Подключение зависимостей в код проекта
Добавьте подключение файла composer с автозагрузкой в ваш файл `init.php`:

```php
require_once __DIR__ . '/vendor/autoload.php';
```

### Доп. материалы
1. [Composer установка](https://getcomposer.org/download/)
2. [Компонент symfony/var-dumper](https://github.com/symfony/var-dumper)


