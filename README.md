# Домашнее задание #3

В качестве домашней работы к 3 заданию Вам необходимо отправить pull request с инструкцией из 2 задания в этот репозиторий, дополнив эту инструкцию командами для работы с удалённым репозиторием. Не забывайте создавать свою ветку под изменения и следите за тем, чтобы терминал был открыт именно в папке Вашего форка. Успехов!

1.  Команда **git add** добавляет содержимое рабочей директории в индекс (staging area) для последующего коммита.
2.  Команда **git status** показывает состояния файлов в рабочей директории и индексе
3.  Команда **git diff** используется для вычисления разницы между любыми двумя Git деревьями.
4. Команда **git commit** берёт все данные, добавленные в индекс с помощью **git add**, и сохраняет их слепок во внутренней базе данных, а затем сдвигает указатель текущей ветки на этот слепок.
5. Команда **git branch** — это своего рода “менеджер веток”. Она умеет перечислять ваши ветки, создавать новые, удалять и переименовывать их.
6. Команда **git checkout** используется для переключения веток и выгрузки их содержимого в рабочую директорию.
7. Команда **git merge** используется для слияния одной или нескольких веток в текущую. Затем она устанавливает указатель текущей ветки на результирующий коммит.
8. Команда **git log** используется для просмотра истории коммитов, начиная с самого свежего и уходя к истокам проекта.
## Удаленный Репозиторий 
1. Команда **git pull** работает как комбинация команд git fetch и git merge, т.е. Git вначале забирает изменения из указанного удалённого репозитория, а затем пытается слить их с текущей веткой.
2. Команда **git push** используется для установления связи с удалённым репозиторием, вычисления локальных изменений отсутствующих в нём, и собственно их передачи в вышеупомянутый репозиторий.