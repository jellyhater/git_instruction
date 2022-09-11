# Домашнее задание #3

В качестве домашней работы к 3 заданию Вам необходимо отправить pull request с инструкцией из 2 задания в этот репозиторий, дополнив эту инструкцию командами для работы с удалённым репозиторием. Не забывайте создавать свою ветку под изменения и следите за тем, чтобы терминал был открыт именно в папке Вашего форка. Успехов!

# Инструкция для работы в Git и с Markdown

## Выделение текста в Markdown

Если вокруг текста сверху и снизу есть пустые строки, то текст превращается в абзац.  
Чтобы сделать перенос строки вместо абзаца,  
нужно поставить два пробела в конце предыдущей строки.

Заголовки отмечаются диезом `#` в начале строки, от одного до шести. Например:

# Заговок первого уровня #
        для этого нужно обрамить заголовок с двух сторон #
## Заголовлоок h2  
        для h2 нужно поставить перед заголовком ##
### Заголовок h3
        для h3 нужно поставить перед заголовком ###
#### Заголовок h4
        для h4 нужно поставить перед заголовком ####
##### Заголовок h5
        для h5 нужно поставить перед заголовком #####
###### Заголовок h6
        для h2 нужно поставить перед заголовком ######

## Списки  
Для разметки неупорядоченных списков можно использовать или `*`, или `-`, или `+`:
* элемент 1
- элемент 2
+ элемент 3

Вложенные пункты создаются четырьмя пробелами перед маркером пункта:
- элемент 1
    - вложенный элемент 1
    + вложенный элемент 2

### Упорядоченный список:

1. элемент 1
2. элемент 2
    1. вложенный
    2. вложенный
3. элемент 3

можно еще проще, надо чтобы перед элементом списка стояла цифра (любая) с точкой.

3. элемент 1
0. элемент 2
12. элемент 3
1980. элемент 4

### Список с абзацами
*   ИТ-специалист — это представитель одной из более чем 500 цифровых профессий, связанных с разработкой программ и использованием компьютерной техники.
*   За 2021 количество вакансий на рынке ИТ выросло на 72%. Количество резюме — всего на 6%

 данное действие делается при помощи 4 пробелов или одного (tab) вначале

Выделять слова можно при помощи `*` и `_`. Одним символ для наклонного текста, два символа для жирного текста, три — для наклонного и жирного одновременно.

Например, это _курсив_ и это тоже *курсив*. А вот так уже __жирный__, и так тоже **жирный**.

 А так ***жирный и наклонный*** одновременно.

зачеркивание текста: две тильды `~` до и после текста.

~~Зачеркнуто~~


### Картинки
Вставить картинку в папку с репозиторией.

![Лунатик](lunatik.jpg)

Не принято сохранять большие файлы, поэтому создаем в папке файл .gitignore и прописываем там имя картинки.
### Ссылки
Это встроенная [ссылка с title элементом](https://gb.ru/ "Я ссылка"). Это — [без title](https://gb.ru/).

А вот [пример][1] [нескольких][2] [ссылок][id] с разметкой как у сносок. Прокатит и [короткая запись][] без указания id.

[1]: https://gb.ru/path-to-it/it_star_08?from=banner_main_path_to_it_urgant_9_26082022 "Optional Title Here"
[2]: https://gb.ru/posts/mincifry-obuchenie
[id]: https://gb.ru/geek_university/developer/programmer (Optional Title Here)
[короткая запись]: https://gb.ru/posts/development

Вынос длинных урлов из предложения способствует сохранению читабельности исходника. Сноски можно располагать в любом месте документа.
### Цитаты
Цитаты оформляются с помощью символа `>`.

> Хотите сделать первый шаг и погрузиться в мир информационных технологий?
Регистрируйтесь на шоу!

> IT-профессии не обязательно обучаться много лет в вузе, но и за несколько месяцев освоить ее невозможно, достаточно 1–1.5 лет, чтобы выйти на уверенный уровень

В цитаты можно помещать всё что угодно, в том числе вложенные цитаты:

> ## Чтобы вы перестали сомневаться в себе
> 
> 1.   В IT не важны склад ума, пол и возраст.
> 2.   В этой сфере работают и гуманитарии, и люди старше 45 лет, и парни, и девушки.
>
> > Главное — постоянно учиться, много практиковаться и быть целеустремленным.

### Работа с GitHub

На GitHub принято, чтобы у каждого проекта был файл read me, то есть файл с описанием того, что происходит внутри проекта. Создадим внутри файл. Но перед этим запомним, когда мы хотим внести или предложить изменения в чей-то проект, это всегда делается *в отдельной ветке*.

Создадим отдельную ветку, а в этой ветке — файл с описанием проекта.
Для начала посмотрим, какие ветки существуют — есть только ветка master. Соответственно, мы можем положить рядом ветку description. У нас появляется новая ветка. Посмотрим, что она действительно появилась. Для этого введём git branch. Перейдём на неё, введя git checkout description. Теперь убедимся, что мы находимся на ней. Далее продолжим работу с этого места: очистим выдачу и создадим новый файл внутри папки group_903. Таким образом, появляется новый файл README.md. Принято называть этот файл сиспользованием клавиши Caps lock, так как это общепринятый способ наименования. Теперь что-нибудь напишем. Просто дадим некоторое описание, это может быть совершенно любой текст: «Это какой-то проект на гитхаб-аккаунте».

Теперь надо всё закоммитить. Для этого добавим указанный файл. Введём git status, чтобы
убедиться, что файл появился, далее прописываем команду add, добавляем файл README.md и git commit. Добавляем некоторое сообщения, например: «Добавили описание к проекту».

Теперь у нас есть основная ветка, в которой происходит работа, и новая. Последней ветки в изначальном репозитории нет, но это именно то, что сейчас требуется. Мы создали
дополнительную ветку, произвели в ней какие-то изменения и хотим предложить их человеку, владеющему основным репозиторием. Для этого направим то, что сделано сейчас, в наш репозиторий. Git как раз подсказывает, что надо набрать, чтобы это сделать. Так как делаем это из соседней ветки, выполним команду git push. Всё можно не запоминать, так как Git почти всегда подсказывает, что надо делать.

Посмотрим на текущее состояние — появилась дополнительная ветка и новая кнопка (Compare
& pull request) на нашем GitHub-аккаунте. Compare — сравнить, pull request — отправь запрос на вливание того, что сделано в основном репозитории. Основным считается тот, что мы взяли — ShafigullinIK/group_903.

Сейчас мы работаем в своём репозитории, а ниже указан чужой репозиторий. Сделали fork И
теперь, когда мы сделали какие-то изменения, добавили новую ветку, можем предложить эти
изменения изначальному хозяину репозитория. Для этого нажимаем на Compare & pull
request.
GitHub проанализировал то, что мы сделали. Он говорит, что можно без проблем слить
сделанное и то, что было в основном репозитории. То есть никаких конфликтов он не
обнаружил и предлагает добавить некоторое описание. В первом поле напишем «Добавили
описание к проекту», а во втором поле добавим информацию «Мы хотели бы помочь вашему
проекту». После этого направим pull request в изначальный аккаунт.

Затем в аккаунте, копию которого мы делали, появляется новое поле. С ним будет работать
уже хозяин этого аккаунта. Он посмотрит на изменения, которые мы сделали. Если
произведённые изменения его устроят, он может влить эту ветку в основной репозиторий.
Именно так происходит работа над проектами open source. Open source — открытый исходный
код, открытый исходник.

Когда группа энтузиастов работает над большим проектом, например, пишет какую-то
программу, сервис, который всем интересен, другие люди могут в этом поучаствовать.
Например, предложить какие-то дополнительные изменения. Это участие осуществляется
именно через систему pull request.

1. Делаем копию аккаунта, который интересен, к себе.
2. Создаём локальный репозиторий, то есть через git clone берём его на свой локальный
компьютер.
3. Создаём ветку, где делаем изменения, которые хотели бы предложить.
4. Направляем свои изменения в собственный аккаунт, и появляется кнопка для
отправки — pull request.

## Создание кнопки pull request

1. Делаем форк (fork) интересующего нас репозитория.
2. Делаем git clone для нашей версии этого репозитория. Так появляется версия на нашем
аккаунте, и именно эту версию мы клонируем.
3. Создаём ветку с предлагаемыми изменениями.
4. Производим все изменения только в этой ветке.
5. Отправляем эти изменения на свой аккаунт (push).
6. В окне на GitHub появляется возможность отправить pull request.
