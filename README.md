# Домашнее задание #3

В качестве домашней работы к 3 заданию Вам необходимо отправить pull request с инструкцией из 2 задания в этот репозиторий, дополнив эту инструкцию командами для работы с удалённым репозиторием. Не забывайте создавать свою ветку под изменения и следите за тем, чтобы терминал был открыт именно в папке Вашего форка. Успехов!
# Команды для работы с github-репозиториями:

Создание локального репозитория
$git clone git@github.com:drnextgis/openlayers.git
$cd openlayers
$git remote add upstream git://github.com/openlayers/openlayers.git

Обновление локального репозитория
$git pull upstream master

Создаем ветку
git checkout -b feature #Создаёт новую ветвь, названную "feature" и делает её активной

Коммиты
$git commit -a -m "message"

Обновление удаленного репозитория
$git push origin feature #Загружает изменения в текущей ветви в origin в ветвь feature

Справочные комманды
$git show
$git log
$git diff

Так же можно удалить ветку, в которой велась разработка:
git branch -d feature #В локальном репозитории
git push origin :feature #В удалённом репозитории