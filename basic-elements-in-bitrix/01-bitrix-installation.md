Начинаем с вами с установки Битрикса. Используйте готовый сервер, если у вас таковой есть. Либо, если хотите запустить проект локально, у вас должны быть установлены `php7.3` или `php7.4` (можно и ниже, но уроки будут построены на этой версии) и `mysql`.

### Скачать Bitrix
Чтобы скачать Битрикс, зайдите на их [сайт в раздел "Скачать"](https://www.1c-bitrix.ru/download/cms.php).

### Запуск с использованием встроенного в php веб-сервера

Для запуска в `PhpStorm` укажите следующие параметры в конфигурации запускаемого приложения:

```text
-d
short_open_tag=on
-d
display_errors=on
-d
mbstring.internal_encoding=utf-8
-d
opcache.revalidate_freq=0
-d
memory_limit=128M
-d
max_input_vars=10000
-d
date.timezone="Europe/Moscow"
-d
sendmail_path="/usr/sbin/sendmail -t -i -f noreply@noserver.ru"
```

Если вы не используете PhpStorm, то выполните подобную такую команду просто из консоли

```shell script
/usr/bin/php7.4 -S course01.bitrixcasts.lesson:8081 -t /www/bitrixcasts/01_course/demo1 -d short_open_tag=on -d display_errors=on -d mbstring.internal_encoding=utf-8 -d opcache.revalidate_freq=0 -d memory_limit=128M -d max_input_vars=10000 -d date.timezone=Europe/Moscow -d "sendmail_path=/usr/sbin/sendmail -t -i -f noreply@noserver.ru"
```

Я использую в уроках доменное имя `course01.bitrixcasts.lesson` и порт `8081` вы можете выбрать другие значение.  Но в любом случае их нужно указать в файле `hosts`

Добавьте туда подобную строку, тем самым вы подскажете вашему компьютеру, что все запросы к этому доменному имени нужно перебрасывать на адрес локального компьютера, а не искать где-то в вебе:

```text
127.0.1.1   course01.bitrixcasts.lesson
```

### Установка Bitrix
Сейчас вы станете свидетелем самого искрометного описания для урока: "Далее просто следуйте мастеру установки."

### Доп. материалы
1. [Документация: Битрикс по процессу установки](https://dev.1c-bitrix.ru/learning/course/index.php?COURSE_ID=32&CHAPTER_ID=04862&LESSON_PATH=3903.4862)

