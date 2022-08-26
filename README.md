# Домашнее задание #3

В качестве домашней работы к 3 заданию Вам необходимо отправить pull request с инструкцией из 2 задания в этот репозиторий, дополнив эту инструкцию командами для работы с удалённым репозиторием. Не забывайте создавать свою ветку под изменения и следите за тем, чтобы терминал был открыт именно в папке Вашего форка. Успехов!

Инструкция по Git (2 урок):  
1. Работу с ветками начинаем с команд git init и git status. Первое чтобы создать репозиторий, а второй чтобы определить статус файла.  
2. Повторяем команды git add, git commit, git log.  
3. Первая команда с которой мы познакомимся, это git branch. С помощью этой команды мы можем узнать сколько веток в нашем репозитории и на какой ветке мы находимся.  
Создать ветку мы можем командой git branch Название ветки.  
4. Если хотите переключиться между ветками, ведите команду git checkout Название ветки.   
5. Если вы захотите слить ветки, то ваш понадобится вести команду git merge Название ветки с которой хотите слить основную ветку.  
6. Если вам больше не нужна одна из созданной вами веток, воспользуйтесь командой git branch -d Название ветки ,которую хотите удалить.  
7. Порой случается конфликт между ветками, которые вы слили. Например, когда на одной и той же строке написанны разные предложения в разных ветках. Как и в жизни любой конфликт можно разрешить с помощью компромисов. Git сам поможет вам разрешить конфликт. Для этого он попросить воспользоваться опцией Система управление версиями или горячими клавишами Ctrl+Shift+G. После того как перейдёте, вам будут даны несколько вариантов решения. С помощью галочек вы можете выбрать какой именно вам подходит.   
8. Если захотите посмотреть на свои коммиты(сохранения) в виде дерева, ведите команду git log --graph.  
   
Работа с удалённым репозиторием:  
Для начала зарегистрироваться на сайте GitHub.
1. Копировать на свой компьютер удаленный или внешний репозиторий из сайта с помощью командф git clone Ссылка репозитория ,которого хотите копировать.
2. Вы скопировали репозиторий, а теперь вам надо выкачать всё содержимое из него. Для этого используем команду git pull.
3. Если же хотите отправить свою версию репозитория в удаленный, тогда вам надо будет вести команду git push. Сам VSC поможет вам вести правильную команду git push после его ввода. Однако при первом его использовании нужна авторизация. 
4. Также существует такое понятие как pull request. Это команда для предложения изменений и запрос на их внесение. Предлагать изменения на GitHub нужно в отдельной ветке. Сначала вы копируете репозиторий на свой компьютер, делаете fork репозитория, затем клонируете версию на своём ПК, создаёте ветку с предлагаемыми изменениями, отправляете изменения командой push в свой аккаунт на GitHub и даёте команду pull request.

На этом всё!