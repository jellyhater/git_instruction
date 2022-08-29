# Краткая инструкция по использованию git

## Полезные ссылки
* [Документация по git. Установка](https://git-scm.com/book/ru/v2/%D0%92%D0%B2%D0%B5%D0%B4%D0%B5%D0%BD%D0%B8%D0%B5-%D0%A3%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B0-Git)
* [Синтаксис языка Markdown от его создателя Джона Грубера](https://daringfireball.net/projects/markdown/syntax)
* [Справочник по Markdown от Microsoft](https://docs.microsoft.com/ru-ru/contribute/markdown-reference)

## Основные команды git

**git init** - инициализация локального репозитория

**git status** - получить информацию от git о его текущем состоянии

Пример:
```
$ git status
```
- В случае, если файл не был изменен:
![git_status_clean](images/git_status_clean.png)
- Если есть незакомиченные изменения:
![git_status_modified](images/git_status_modified.png)

**git add** - добавить файл или файлы к следующему коммиту

Пример:
```
$ git add git_readme.md 
```
![git_add](images/git_add.png)

**git commit -m “message”** - создание коммита

Пример:
```
$ git commit -m "Added main git commands"
```
![git_commit](images/git_commit.png)

**git log** – вывод на экран истории всех коммитов с их хеш-кодами

Пример:
```
$ git log
```
![git_log](images/git_log.png)

**git checkout [хеш-код]** – переход от одного коммита к другому (достаточно ввести первые 4 символа хэш-кода коммита)

Пример:
```
$ git checkout cdcd
```
![git_checkout](images/git_checkout.png)
+ Результат выполнения:
![git_checkout_cdcd](images/git_checkout_result.png)

**git checkout master** – вернуться к актуальному состоянию и продолжить работу

Пример:
```
$ git checkout master
```
![git_checkout_master](images/git_checkout_master.png)
+ Результат выполнения:
![git_checkout_master_res](images/git_checkout_master_result.png)

**git diff** – увидеть разницу между текущим файлом и закоммиченным файлом

Пример:
```
$ git diff
```
![git_diff](images/git_diff.png)

## Работа с удаленными репозиториями

### 1. Создание удаленного репозитория из локального репозитория.
+ Создать локальный репозиторий  
    - **git init**, **git add**, **git commit**
+ Создать репозиторий на GitHub (пустой, без README.md файла), например, MyFirstRepo.
    - После создания удаленного репозитория GitHub подскажет, что на локальном репозитории надо выполнить следующие команды:
        * **git remote add origin https://username/MyFirstRepo.git**
        * **git branch -M main**
        * **git push -u origin main**
+ Выполнить указанные выше команды в локальном репозитории после коммита
+ Далее для обновления удаленного репозитория достаточно выполнять **git push**

### 2. Копирование удаленного репозитория в локальный.
Для копирования удаленного репозитория в локальный необходимо:
+ На удаленном репозитории через кнопку Code скопировать https ссылку на репозиторий, например это будет https://username/MyFirstRepo.git
+ Открыть пустую папку, где нет git репозитория (**git status** выдаст fatal error: no repository)
+ Выполнить в терминале **git clone https://username/MyFirstRepo.git**
+ Перейти в папку с репозиторием через команду **cd**.

### 3. Создание pull request для репозитория другого пользователя.
+ Делаем форк (fork) интересующего нас репозитория в свой GitHub аккаунт.
+ Делаем git clone для нашей локальной версии этого репозитория.
+ Создаем ветку с предлагаемыми изменениями в локальном репозитории.
+ Производим все изменения только в этой ветке.
+ Отправляем все эти изменения на свой аккаунт (push).
+ В окне Github появляется возмжность отправить pull request через созданную ветку внутри fork-репозитория.
