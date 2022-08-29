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
