<div id="header" align="center">
    <img src="https://media.giphy.com/media/M9gbBd9nbDrOTu1Mqx/giphy.gif" width="100"/>
    <div id="badges">
    <a href="https://git-scm.com/">
        <img src="https://img.shields.io/badge/GitScm-orange?logo=git&logoColor=white&style=flat" alt="git"/>
    </a>
    <a href="https://www.youtube.com/watch?v=SEvR78OhGtw&list=WL&index=13&t=15s">
        <img src="https://img.shields.io/badge/Youtube-red?logo=youtube&logoColor=white&style=flat" alt="youtube"/>
    </a>    
    </div>  
</div>


# **Установка Git и Visual Studio Code**
1. Установка Git для Windows, MAC, Linux: https://git-scm.com/downloads
2. Установка VSCode для Windows, MAC, Linux: https://code.visualstudio.com/Download

При первом использовании Git необходимо представиться. 
Для этого нужно ввести в терминале 2 команды:
* ***git config --global user.name*** *«ваше имя английскими 
буквами»* 
_Пример:_ 
    >git config levchenko.vg
* ***git config --global user.email*** *«ваша почта@example.com»*
_Пример:_         
    >git config levchenko.vg@gmail.com

_Дополнительную информацию о конфигурации Git можно прочитать_ 
[**тут**](https://git-scm.com/book/ru/v2/%D0%9D%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B9%D0%BA%D0%B0-Git-%D0%9A%D0%BE%D0%BD%D1%84%D0%B8%D0%B3%D1%83%D1%80%D0%B0%D1%86%D0%B8%D1%8F-Git)

# **Основные команды Git** 

* *git init* – инициализация локального репозитория
* *git status* – получить информацию от git о его текущем 
* состоянии
* *git add* – добавить файл или файлы к следующему коммиту
* *git commit -m “message”* – создание коммита.
* *git log* – вывод на экран истории всех коммитов с их хеш-кодами
* *git checkout* – переход от одного коммита к другому
* *git checkout master* – вернуться к актуальному состоянию и продолжить работу
* *git diff* – увидеть разницу между текущим файлом и закоммиченным файлом

_Подробнее о системе контроля версии можно почитать_ [**тут**](https://git-scm.com/book/ru/v2/%D0%92%D0%B2%D0%B5%D0%B4%D0%B5%D0%BD%D0%B8%D0%B5-%D0%9E-%D1%81%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D0%B5-%D0%BA%D0%BE%D0%BD%D1%82%D1%80%D0%BE%D0%BB%D1%8F-%D0%B2%D0%B5%D1%80%D1%81%D0%B8%D0%B9)


![git](git-kod-kaynak-yonetimi-ogrenmek-istiyorum.png)



#
# **Шпаргалка по markdown**

## **Заголовки**

# H1
## H2
### H3
#### H4
##### H5
###### H6

## **Начертание**
Курсив обозначается одинарнимы *звездочками* или _подчеркиваниями_.
Полужирный текст обозначаается двойными **звёздочками** или __подчеркиваниями__.
Для нужно начертания можно комбинировать **звёздочки и _подчеркивания_**.
Две тильды перечёркивают текст. ~~Перечеркнутый текст~~

## **Списки**
1. Первый элемент в нумерованном списке
2. Следующий элемент
  * Элемент ненумерованного списка. 
1. Номер элемента определяется автоматически, главное вставить какую-то цифру
  1. Нумерованный подсписок
4. Ещё один элемент  

Пример текста, который должен быть выровнен по элементу №4 

* Ненумерованный список может использовать звёздочки
- Или минусы
+ Или плюсы

## **Ссылки**
Есть 2 способа создать ссылку:

[С указанием ссылки сразу](https://www.google.com)

[С указанием ссылки в сноске][Arbitrary case-insensitive reference text]

[Можно использовать цифры в качестве сносок][1]

Также любая ссылка, обрамлённая в угловые скобки, автоматом преобразуется
<https://www.google.com>

Какой-то текст перед сносками

[arbitrary case-insensitive reference text]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com

## **Изображения**
Задаются почти также, как и ссылки (2 способа)

Задание ссылки на изображения сразу: 
![alt text](https://k50.ru/img/logos/logo_on_red.png "Logo Title Text 1")

Указание ссылки на изображение в сноске: 
![alt text][logo]

[logo]: https://k50.ru/img/logos/logo_on_red.png "Logo Title Text 2"

## **Подсветка кода и выделение элементов**
С помощью апострофов `текст` будет `обрамлён`.

Большие куски кода обрамляются тройными апосторофами (возникли сложности с отображением синтаксиса - всё автокомментится, поэтому где-то вместо трёх апострофов немного больше)
При добавлении префикса языка программирования будет меняться подсветка.

```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```
```python
s = "Python syntax highlighting"
print s
```
```
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
``` 

## **Таблицы**
Обязательно требуют заголовок и настройки выравнивания (второй строкой). Выравнивание задаётся двоеточием. Колонки задаются вертикальным палками (|)

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

Внешние вертикальные палки (|) задавать необзяательно, также не требуется подгонять колонки под один размер. Можно использовать стили, описанные выше.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3

test