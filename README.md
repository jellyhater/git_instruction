# Домашнее задание #3

В качестве домашней работы к 3 заданию Вам необходимо отправить pull request с инструкцией из 2 задания в этот репозиторий, дополнив эту инструкцию командами для работы с удалённым репозиторием. Не забывайте создавать свою ветку под изменения и следите за тем, чтобы терминал был открыт именно в папке Вашего форка. Успехов!

# Основные команды Git #

1.  **git init** – инициализация локального репозитория
2. **git status** – получить информацию от git о его текущем состоянии
3. **git add** – добавить файл или файлы к следующему коммиту
4. **git commit -m “message”** – создание коммита.
5. **git log** – вывод на экран истории всех коммитов с их хеш-кодами
6. **git checkout** – переход от одного коммита к другому
7. **git checkout master** – вернуться к актуальному состоянию и продолжить работу
8. **git diff** – увидеть разницу между текущим файлом и закоммиченным файлом

~~Ошибок быть не должно~~

![Сразу было страшно начинать а потом оказалось очень интересно](https://myslide.ru/documents_7/fbc5a6c395223dc8c49b208bbcffcfec/img15.jpg)

Урок 2 достаточно информативный, но на семинаре который я смотрела в записи не получилось смержить конечный результат, посмотрим получится ли в домашке это.
 
Есть ветка мастер, к ней добавили ветка_2

На третьей ветке делаю конфликт в 20 строку между мастер и ветка_3

Получилась красота даже луше чем ожидала, значит на семинаре где-то ошибка была

# Дополнение к инструкции 

Команда **git clone** составная: она не только загружает все изменения, но и пытается слить все ветки на локальном компьютере и в удаленном репозитории.

**git pull** - эта команда позволяет скачать все из текущего репозитория и автоматически 
сделать merge с нашей версией.

**git push** - позволяет отправить нашу версию репозитория на внешний репозиторий. ТРЕБУЕТ АВТОРИЗАЦИИ на внешнем репозитории.