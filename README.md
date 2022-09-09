# Домашнее задание #3

В качестве домашней работы к 3 заданию Вам необходимо отправить pull request с инструкцией из 2 задания в этот репозиторий, дополнив эту инструкцию командами для работы с удалённым репозиторием. Не забывайте создавать свою ветку под изменения и следите за тем, чтобы терминал был открыт именно в папке Вашего форка. Успехов!

# Инструкция для работы с Markdown

## Выделение текста

Чтобы выделить текст курсивом необходимо обрамить его звездочками (*) или знаком (_). Например, *вот так* или _вот так_.

Чтобы выделить текст полужирным необходимо обрамить его двойными звездочками (**) или двойным знаком нижнего подчеркивания (__). Например, **вот так** или __вот так__.

Альтернативные способы выделения текста жирным или курсивом нужны для того, чтобы мы могли совмещать оба этих способа. Например, _текст может быть выделен курсивом и при этом  быть **полужирным**_.

## Списки
Чтобы добавить ненумерованные списки необходимо пункты выделить звездочкой (*) или знаком (+). Например, вот так:
* Элемент 1
* Элемент 2
* Элемент 3
+ Элемент 4

Чтобы добавить нумерованные списки необходимо пункты просто пронумеровать. Например, вот так:
1. Первый пункт
2. Второй пункт 1111111
## Работа с изображениями

Чтобы вставить изображение в текст достаточно написать следующее: ![Привет, это Билли!](unnamed.jpg)
## Ссылки
В ваши документы можно вставлять и ссылки на страницы в интернете. Делается это вот так: [заголовок_ссылки](сама_ссылка):

[Google](google.com)

Аналогично в документ вставляются и изображения. Поставьте восклицательный знак, подпись к изображению в квадратных скобках и ссылку на него в круглых скобках. Можно указывать ссылки на картинки как из интернета, так и на хранящиеся на жёстком диске. Подпись указывать необязательно. Выглядит это следующим образом:

![подпись](ссылка_на_изображение) 11111111

Эскапированные символы
Иногда вам нужно вставить в документ какой-нибудь символ, который относится к синтаксису Markdown. Вы печатаете его, и форматирование меняется, хоть вам это и не нужно. В таком случае перед техническими символами нужно ставить обратный слэш — \.


## Таблицы
Если ваш редактор поддерживает GFM, то в нём можно создавать простенькие таблицы. Для таблиц используйте символы | и -. Примерно так:

| раз | два | три |
|:----|:----|:----|
| раз | два | три |

Списки дел
В Markdown есть даже своеобразные списки задач — аналог чекбоксов в OneNote или Evernote. Вот как они выглядят:

- [ ] Невыполненная задача
- [ ] Невыполненная задача
- [X] Выполненная задача



## Цитаты

Иногда какой-то абзац нужно выделить как цитату. В этом случае воспользуйтесь знаком >. Его необходимо проставлять перед каждой строчкой цитаты.

> Очень глубокомысленная цитата. Пожалуйста, прочтите её внимательно.
>
> Оскар Уайльд

## Работа с удаленными репозиториями

Как сделать pull request

- Делаем (ответвление) fork репозитория
- Делаем git clone СВОЕЙ версии репозитория
- Создаем новую ветку и в НЕЕ вносим свои изменения
- Фиксируем изменения (делаем коммиты)
- Отправляем свою версию в свой GitHub
- На сайте GitHub нажимаем кнопку pull request