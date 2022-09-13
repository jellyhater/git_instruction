# Домашнее задание #3

В качестве домашней работы к 3 заданию Вам необходимо отправить pull request с инструкцией из 2 задания в этот репозиторий, дополнив эту инструкцию командами для работы с удалённым репозиторием. Не забывайте создавать свою ветку под изменения и следите за тем, чтобы терминал был открыт именно в папке Вашего форка. Успехов!

***

***

***


## Команды Git
***
+ **git init** - *инициализация репозитория*;
+ **git add** - *добавить файл к коммиту*;
+ **git commit -m "comment"** - *создание коммита с комментарием*;
+ **git status** - *запрос состояния репозитория*;
+ **git log** - *список коммитов*;
+ **git diff** - *отображение изменений текущего файла с файлом коммита*;
+ **git checkout 4_chars** - *переход к коммиту по 4 символам хэша*;
+ **git checkout master** - *возврат к актуальному состоянию*.
***
Список команд Git по первой лекции и семинару.

***
***
### Ветвление

+ **git branch** - посмотреть ветку (со звездой текущая)

+ **git branch <new_name>** - создать ветку

+ **git checkout <name>** - перейти на ветку

+ **git merge <имя папки слияния с текущей>** - объединение

+ **git branch -d <name>** - удаление ветки

***
Список команд Git по второй лекции и семинару.

***
***
### Работа с удаленным репозиторием

+ **git clone https://…** - скопировать репозиторий на локальный комп

+ **git remote add origin https://…** - связываем локальный и удаленный репозиторий

+ **git branch -M main** - указываем какая ветка является главной

+ **git push -u origin main** - направляем из локального репозитория на удаленный

+ **git push** - загрузить на github (затолкать)

+ **git pull** - скачать с github (стянуть)

***

+ Делается fork интересующего проекта.
+ git clone - для копирования "нашей" версии этого репозитория.
+ Создается новая ветка с предлагаемыми изменениями.
+ Отправляются изменения на свой аккаунт git push --set-upstream origin description
+ В окне на GitHub появляется возможность отправить автору Pull&Request.

***
Список команд Git по третьей лекции.

***
***

> Подробнее [на Wiki](https://en.wikipedia.org/wiki/Git)