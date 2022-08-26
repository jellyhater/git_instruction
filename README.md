# Домашнее задание #3

В качестве домашней работы к 3 заданию Вам необходимо отправить pull request с инструкцией из 2 задания в этот репозиторий, дополнив эту инструкцию командами для работы с удалённым репозиторием. Не забывайте создавать свою ветку под изменения и следите за тем, чтобы терминал был открыт именно в папке Вашего форка. Успехов!

# **Git и работа с ним**

**Git** — система контроля версий *(файлов)*.
Что-то вроде возможности сохраняться в компьютерных играх

**Коммит** — «сохранение»
*(хранит набор изменений, сделанный в рабочей директории с
момента предыдущего коммита)*.

 ## **Простейший цикл работ:**

 * Редактирование 

 * Добавление

 * Удаление файлов (собственно, работа)

 * Индексация/добавление файлов в индекс *(указание для git
    какие изменения нужно будет закоммитить)*

 * Коммит *(фиксация изменений)*

 * Возврат к шагу 1


### **Перед началом работы нужно выполнить некоторые настройки:**

1. **git config --global user.name "Указать имя"**

2. **git config --global user.email "Указать почту"**

3. **git init (Включить отслеживание папки)**

### **Для сохранения и фиксациии зменений:**

1. Ctrl + S *(Сохранить локально)*

2. git add _имя файла_

3. git commit -m"_Комментарий_"

## **Команды GIT:**

* *git status* - **показать статус**

* *git log* - **показать этапы фиксации**

* *git checkout _имя_* - **переход от одного коммита к другому**

* *git diff* – **увидеть разницу между текущим файлом и закоммиченным файлом**

* *git checkout master* – **вернуться к актуальному состоянию и продолжить работу**

* *git branch* - **показать список веток**

* *git branch new_branch* - **создать новую ветку с указанным именем на текущем коммите**

* *git branch -d existing_branch_name* - **удаление ветки**


# Работа с GITHUB

Для того чтобы начать работу с удаленными репозиториями, надо создать аккаунт на GitHub.
Затем надо создать новый репозиторий и следаоать инструкциям, которые предоставляет платформа.
Для того чтобы работать с чужим репозиторием надо открыть репозиторий на сайте GitHub и воспользоваться кнопкой Fork в правом верхнем углу.

В результате мы получим удаленный репозиторий у себя в аккаунте GitHub.
Далее надо "стянуть" или клонировать этот репозиторий воспользовавшись ссылкой со страницы репозитория и командой

**git clone <адрес>**

Результатом этой комнды будет копия репозитория на локальном компьютере. Далее создаем новую ветку и переходим на нее.
Добавив все необходимые изменения, создаем коммит и вводим в терминале команду:

**git push**

Эта команда позволяет залить изменения на удалённый репозиторий.
Так как ветка создана только локально git предложит нам ее добавить и посоветует как это сделать.
При переходе по этим ссылкам открывается окно, в котором можно отправить свой request и добавить к нему комментарий.