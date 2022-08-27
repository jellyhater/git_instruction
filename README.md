# Домашнее задание #3

# Инструкция по работе с GIT
(этот текст написан в файле с языком разметки Markdown и с разными его примочками)

Перед началом работы нужно выполнить некоторые настройки:

git config --global user.name "Your Name" # указать имя, которым будут подписаны коммиты
git config --global user.email "e@w.com"  # указать электропочту, которая будет в описании коммите

Вот здесь много команд:
https://github.com/cyberspacedk/Git-commands

А здесь советы про git:
https://gb.ru/posts/soveti-pro-git 

**NB! Программу Git создал Линус Торвальдс, который стоял за созданием системы Linux.**

## git init
Команда, которая вводится в самом начале. Создание локального репозитория, начало отслеживания изменений.  
Нужно вводить после выбора папки, в которой хочется создать репозиторий. *Куда вводить? В терминал! Который можно вывести с помощью верхнего меню (соответствующее слово или через вкладку "Вид"). Также можно использовать горячие клавиши для его вывода с лямбдой.*  
NB! На будущее надо всегда помнить про локальные сохранения (СMD + S). Если изменения не сохранены, то рядом с названием файла висит белый кружочек.

## git add
Команда, которая добавляет файлу версионность. Команда, которую нужно вводить после добавление файлов/изменений в файл для последующих коммитов. После git add надо ввести название файла с расширением. Не обязательно печатать его самостоятельно, достаточно воспользоваться табом после первых пары символов. NB! Не забывай про сохранение;)

## git commit
Команда, которая позволяет зафиксировать, сохранить и добавить комментарий к текущей версии, которая была "слеплена" из git add. Сам комментарий добавляется через **-m "В кавычках должен быть написан комментарий"**.

## git log
Команда, которая позволяет вывести журнал изменений со всеми комментариями к ним. Если вдруг терминал вывел только пару последних изменений, то надо воспользваться стрелочками на клавиатуре для перемещения между ними.

## git checkout
Команда, которая позволяет переключаться между версиями. Для работы **после ввода команды надо указать интересующий коммит (первых 4+ цифр будет достаточно)**.  
Вернуться в рабочий коммит можно с помощью **git checkout master**.  
*Кстати!* Нажатие клавиши q возвращает в исходное окно терминала.

## git diff
Команда, которая показывает разницу между текущим файлом и сохранённым.

## git branch
Команда, которая позволяет выводить список имеющихся веток. Условно, это черновики или отдельные куски работы, которые потом можно слить в единое целое.

## git branch название_ветки
Создание новой ветки.

## git branch -d название_ветки
Команда, которая позволяет удалить ненужную ветку. 

## git merge название_ветки
Команда, которая позволяет сливать две ветки. Надо запускать из той ветки, в которую хочется слить, а писать название той ветки, которую хочется "влить" в другую.

Тренажер для обучения гиту: https://learngitbranching.js.org/?locale=ru_RU


## Инструкция по работе с удалённым репозиторием

1. На GitHub делаем Fork нужного репозитория. 
2. У себя в аккаунте берём ссылку этого форка (Зеленая кнопка "CODE") копируем с расширением HTTPS
3. Создаём папку с любым названием и открываем её в VS code.
4. Делаем клон репозитория командой в терминале **git clone ссылка_на_репо**
5. Внутри созданной и открытой папки появится клонированный репозиторий. Учитель советует открыть нужный файл отдельно в VS code, но можно воспользоваться командой **cd название папки**, чтобы переключиться на нужную дерикторию.
6. В терминале обязательно создаём новую ветку. Это вежливость! **git branch new_branch_name**.
7. Переходим на новую ветку **git checkout name_branch_name**.
8. Вносим необходимые изменения в этой ветке.
9. Сохраняем, добавляем в add, прописываем **git commit -m "Любой текст для понимания, что сохранено"**.
10. Теперь можно пушиться:)) В терминале прописываем **git push --set-upstream origin name_branch**. Можно просто **git push**, а потом скопировать, что надо. 
11. Переходим в GitHub и делаем там то, что надо.
12. Кстати, чтобы "стянуть" все обновления из удалённого репозитория, надо выводить команду **git pull**. Эта команда не только подгружает, но и мёржит!