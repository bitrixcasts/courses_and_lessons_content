### 1. Инициализация git
Проинициализируйте **git** репозиторий, выполнив следующую команду в корне проекта:

```shell script
git init
```

### 2. Настройка .gitignore
Отредактируйте файл **.gitignore**, добавьте в него следующее содержимое:

```text
bitrix
upload
.idea
```

### 3. Опция filemode
*Опционально.* Отредактируйте настройки git репозитория, отмените слежение за правами на файлы отменив опцию `filemode`

```shell script
git config core.filemode false
```

Или вручную отредактируйте файл **.git/config**

```text
[core]
    ...
    filemode = false
...
```

### 4. Первый коммит
Зафиксируйте изменения, добавив все файлы под индекс
```shell script
git add .
git commit -m'Initial Commit'
```

### 5. Profit