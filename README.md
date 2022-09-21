# Домашнее задание #3

В качестве домашней работы к 3 заданию Вам необходимо отправить pull request с инструкцией из 2 задания в этот репозиторий, дополнив эту инструкцию командами для работы с удалённым репозиторием. Не забывайте создавать свою ветку под изменения и следите за тем, чтобы терминал был открыт именно в папке Вашего форка. Успехов!

Домашнее задание 3

# Основные команды Git
- git init – инициализация локального репозитория
- git status – получить информацию от git о его текущем состоянии
- git add – добавить файл или файлы к следующему коммиту
- git commit -m “message” – создание коммита.
- git log – вывод на экран истории всех коммитов с их хеш-кодами
- git checkout – переход от одного коммита к другому
- git checkout master – вернуться к актуальному состоянию и продолжить работу
- git diff – увидеть разницу между текущим файлом и закоммиченным файлом

**Если вы не до конца настроили систему для работы, в начале своего пути - не беда. Git всегда подскажет разработчику, если тот запутался, например:**

1. Команда git --help - выводит общую документацию по git
2. Если введем git log --help - он предоставит нам документацию по какой-то определенной команде (в данном случае это - log)
3. Если вы вдруг сделали опечатку - система подскажет вам нужную команду
4. После выполнения любой команды - отчитается о том, что вы натворили
5. Также Гит прогнозирует дальнейшие варианты развития событий и всегда направит разработчика, не знающего, куда двигаться дальше


**Домашнее задание 2**

**Работа с Ветками**

- git branch # показать список веток
- git branch -v # показать список веток и текущий коммит в каждой
- git branch new_branch # создать новую ветку с указанным именем на текущем коммите
- git branch new_branch 5589877 # создать новую ветку с указанным именем на указанном коммите
- git branch -f master 5589877  # переместить ветку master на указанный коммит
- git branch -f master master~2 # переместить ветку master на 2 коммита назад
- git checkout new_branch    # перейти в указанную ветку
- git checkout -b new_branch # создать новую ветку с указанным именем и перейти в неё
- git checkout -B master 5589877 # переместить ветку с указанным именем на указанный коммит и перейти в неё
- git merge hotfix # влить в ветку, в которой находимся, данные из ветки hotfix
- git merge hotfix -m "Горячая правка" # влить в ветку, в которой находимся, данные из ветки hotfix (указано сообщение коммита слияния)
- git merge hotfix --log  # влить в ветку, в которой находимся, данные из ветки hotfix, показать редактор описания коммита, добавить в него сообщения вливаемых коммитов
- git branch -d hotfix       # удалить ветку hotfix (используется, если её изменения уже влиты в главную ветку)
- git branch --merged        # показать ветки, уже слитые с активной
- git branch --no-merged     # показать ветки, не слитые с активной
- git branch -a              # показать все имеющиеся ветки (в т.ч. на удаленных репозиториях)

**Работа с удаленными репозиториями**

- заходим в личный кабинет на github
- создаем репозиторий или заходим в существующий
- прееходим по ссылке на нужный репозиторий
- делаем форк этого репозитория
- копируем ссылку в форке
- заходим в вс код, в любую папку (создаем новую или заходим в уже имеющуюся)
- находясь в папке открываем терминал и вводим команду git clone и ссылку на форк удаленного репозитория
- создаем новую ветку
- вносим изменения в файл
- вводим команду git add и git commit
- затем делаем pull request