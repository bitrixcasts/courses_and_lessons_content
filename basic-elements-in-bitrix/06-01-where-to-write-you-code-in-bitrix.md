Создаем файл `/local/php_interface/init.php`.
### Файл init.php
Этот файл является входной точкой для вашего кода в приложении.

Файл `init.php` подключается каждый раз, когда стартует ядро битрикса.

#### Пример функции для отладки кода
```php
function dd(...$data)
{
    echo '<pre>';
    var_dump(...$data);
    echo '</pre>';
    die;
}
```

### Доп. материалы
1. [Документация: Файл init.php](https://dev.1c-bitrix.ru/learning/course/index.php?COURSE_ID=43&LESSON_ID=2916&LESSON_PATH=3913.4776.2916)