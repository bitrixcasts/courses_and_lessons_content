Среди всех файлов разделов внутри вашего файла есть только три системные директории: `bitrix`, `local`, `upload`. Остальные папки только - страницы вашего сайта.

#### Директория local
Папка `local` - частично повторяет структуру папки `bitrix`

**! Важно !**
Разрабатывайте свой код только в директории `local`

### Создание страниц и разделов
#### Создание в административном разделе
В разделе `Контент -> Файлы и папки` Добавляем новый раздел

Название раздела `example1`

Тело индексной страницы:
```text
Hello World
```  
Таким образом будет создана примерно следующая страница:
```php
<?
require($_SERVER["DOCUMENT_ROOT"]."/bitrix/header.php");
$APPLICATION->SetTitle("Example 1");
?>
Hello World
<?require($_SERVER["DOCUMENT_ROOT"]."/bitrix/footer.php");?>
```

#### Создание раздела вручную
Создаем директорию в корне проекта с названием `example2`

Внутри нее создаем файл `index.php`, со следующим содержимым:
```php
<?php
require $_SERVER['DOCUMENT_ROOT'] . '/bitrix/header.php';
?>
Hello World 2
<?php
require $_SERVER['DOCUMENT_ROOT'] . '/bitrix/footer.php';

```
### Доп. материалы
1. [Документация: Структура файлов](https://dev.1c-bitrix.ru/learning/course/index.php?COURSE_ID=43&LESSON_ID=2287&LESSON_PATH=3913.4608.2287)


