# Язык синтаксиса Markdown

## Блочные элементы

### Параграфы и разрвывы строк

Для того, чтобы создать параграф с использованием синтаксиса языка Markdown, достаточно отделить строки текста одной (или более) пустой строкой (пустой считается   всякая строка, которая не содержит в себе ничего, кроме пробелов и символов табуляции). Для того, чтобы вставить видимый перенос строки необходимо окончить строку двумя пробелами и нажатием клавиши «Enter». Многие элементы синтаксиса Markdown выглядят и работают гораздо лучше в случае, когда их форматируют с помощью «жесткого перевода строк» (разделение строк, осуществленное самим пользователем, а не программой автоматически). К таким элементам относятся цитаты, списки и пр.

### Заголовки

Язык разметки Markdown поддерживает 2 стиля обозначения заголовков: подчеркивание и выделение символом («#»). Выделение заголовков с помощью подчеркивания производится знаками равенства («=») в случае, если заголовок первого уровня, и дефисами («-») в случае, если заголовок второго уровня. Количество знаков подчеркивания не ограничивается. При выделении заголовков с помощью символа («#») используется от одного до шести данных символов, которые устанавливаются в начале строки (перед заголовком). В данном случае количество символов соответствует уровню заголовка. Кроме того, заголовок возможно снабдить закрывающимися символами («#»), хотя это и не является обязательным. Количество закрывающихся символов не обязано соответствовать количеству начальных символов. Уровень заголовка определяется по количеству начальных символов.
Выполнение заголовков с помощью символа (#), выглядит следующим образом:

```

1 <#> Заголовок 1 уровня

2 <##> Заголовок 2 уровня

```
  
### Цитаты

Для обозначения цитат в языке Markdown используется знак «больше» («>»). Его можно вставлять как перед каждой строкой цитаты, так и только перед первой строкой параграфа. Также синтаксис Markdown позволяет создавать вложенные цитаты (цитаты внутри цитат). Для их разметки используются дополнительные уровни знаков цитирования («>»). Цитаты в Markdown могут содержать всевозможные элементы разметки. Цитаты в языке Markdown выглядят следующим образом:

```
>Это пример цитаты,
>в которой перед каждой строкой
>ставится угловая скобка.

>Это пример цитаты,
в которой угловая скобка
ставится только перед началом нового параграфа.
>Второй параграф.
```
Вложение цитаты в цитату выглядит следующим образом:
```
> Первый уровень цитирования
>> Второй уровень цитирования
>>> Третий уровень образования
> 
>Первый уровень цитирования
```

В результате на экран выводится следующее:

> Это пример цитаты, в которой перед каждой строкой ставится угловая скобка.

>Это пример цитаты,в которой угловая скобка ставится только перед началом нового параграфа.

>Второй параграф.

Вложенная цитата:

> Первый уровень цитирования
>> Второй уровень цитирования
>>> Третий уровень цитирования
>
>Первый уровень цитирования

### Списки

Markdown поддерживает упорядоченные (нумерованные) и неупорядоченные (ненумерованные) списки. Для формирования неупорядоченный списков используются такие маркеры, как звездочки, плюсы и дефисы. Все перечисленные маркеры могут использоваться взаимозаменяемо. Для формирования упорядоченных списков в качестве маркеров используются числа с точкой. Важной особенностью в данном случае является то, что сами номера, с помощью которых формируется список, не важны, так как они не оказывают влияния на выходной HTML код. Как бы ни нумеровал пользователь список, на выходе он в любом случае будет иметь упорядоченный список, начинающийся с единицы (1, 2, 3…). Эту особенность стоит учитывать в том случае, когда необходимо использовать порядковые номера элементов в списке, чтобы они соответствовали номерам, получающимся в HTML. Упорядоченные списки всегда следует начинать с единицы. Маркеры списков обычно начинаются с начала строки, однако они могут быть сдвинуты, но не более чем на 3 пробела. За маркером должен следовать пробел, либо символ табуляции. При необходимости в список можно вставить цитату. В этом случае обозначения цитирования ( «>» ) нужно писать с отступом. 

Упорядоченные списки выглядят следующим образом:

```
1. Список
2. Список
3. Список
```

Неупорядоченные списки выглядят следующим образом:

```
* Список
* Список
* Список
```

### Разделительные линии

Для того чтобы создать горизонтальную линию с использованием синтаксиса языка Markdown, необходимо поместить три (или более)дефиса или звездочки на отдельной строке текста. Между ними возможно располагать пробелы. 

Горизонтальные линии в Markdown выглядят следующим образом:

```
Первая часть текста, который необходимо разделить
*** или ___
Вторая часть текста, который необходимо разделить
```

В результате на экран выводится следующее:

Первая часть текста, который необходимо разделить
___

Вторая часть текста, который необходимо разделить

## Строчные элементы

### Ссылки

Markdown поддерживает два стиля оформления ссылок:

+ Гиперссылка, с немедленным указанием адреса (внутритекстовая);
+ Гиперссылка, подобная сноске.

```
[пример](http://example.com/ "Необязательная подсказка")
```

Подразумевается, что помимо URL-адреса существует еще текст ссылки. Он заключается в квадратные скобки. Для создания внутритекстовой гиперссылки необходимо использовать круглые скобки сразу после закрывающей квадратной. Внутри них необходимо поместить URL-адрес. В них же возможно расположить название, заключенное в кавычки, которое будет отображаться при наведении, но этот пункт не является обязательным.

### Выделение текста

Markdown воспринимает звёздочки «*» и символы подчёркивания «_» как признаки смыслового выделения текста:

- Текст, окружённый одиночными «*» или «_».

- Текст, окружённый двойными «*» или «_».

Иными словами, текст, окруженный одинарными символами, выделяется курсивным шрифтом, а текст, окруженный двойными символами, выделяется полужирным шрифтом. Также, выделенный фрагмент может находиться в любой части слова. Текст, выделенный курсивом с использованием синтаксиса языка Markdown, выглядит следующим образом:

```
*пример*
```
*пример*

```
**пример*
```
**прмер**

### Изображения

В Markdown существует 2 способа вставки изображений в документ:
1. С помощью непосредственного указания URL-адреса изображения. Синтаксис данной команды выглядит следующим образом:

```
![Альтернативный текст](/путь/к/изображению.jpg)
```
или
```
![Альтернативный текст](/путь/к/изображению.jpg "Подсказка")
```
Иными словами, он состоит из следующих элементов:

+ восклицательный знак;

+ квадратные скобки, в которых указывается альтернативный изображению текст (он станет содержимым атрибута в элементе img);

+ круглые скобки, содержащие URL-адрес или относительный путь изображения, а также (необязательно) всплывающую подсказку, заключённуе в двойные или одиночные кавычки.

2. С помощью метки-идентификатора. Синтаксис данной команды записывается следующим образом:

```
![Альтернативный текст][id]
```

где «id» — имя определённой метки изображения. Метки изображений определяются при помощи синтаксиса, совершенно идентичного меткам гиперссылок:

```
[id]: путь/к/изображению "Необязательная подсказка"
```
Важной особенностью является то, что Markdown не позволяет задать размеры изображения (ширину, высоту).

## Дополнительные элементы

### Обратный слеш

Может употребляться в Markdown перед специальными символами для того, чтобы они воспринимались в их буквальном (а не служебном) значении. Полный список данных символов приводится ниже:

```
«\» - слеш;

«`» - обратный апостроф;

«*» - звездочка;

«_» - символ подчеркивания;

«{}» - фигурные скобки;

«[]» - квадратные скобки;

«()» - круглые скобки;

«#» - символ решетки;

«+» - плюс;

«-» - минус (дефис);

«.» – точка;

«!» - восклицательный знак.
```

### Специальные символы HTML

В языке HTML существует два символа, требующих специального рассмотрения: это символы («<») и («&»). Левая угловая скобка используется как начало тэга; амперсанды применяются для обозначения специального символа HTML. Для того чтобы использовать эти символы в их буквальном смысле, необходимо заменить их элементами HTML, а именно (&lt); и (&amp); соответственно. При использовании Markdown подобных действий совершать не нужно. Он позволяет использовать эти символы в исходном виде. В случае если амперсанд используется как часть спецсимвола HTML, он останется неизменным. В противном случае Markdown преобразует его в (&amp);.

# Инструмент pull request

## Алгоритм работы через систему pull request

1. Делаем копию аккаунта, который интересен, к себе.
2. Создаём локальный репозиторий, то есть через git clone берём его на свой локальный компьютер.
3. Создаём ветку, где делаем изменения, которые хотели бы предложить.
4. Направляем свои изменения в собственный аккаунт, и появляется кнопка для
отправки — pull request.

## Создание кнопки pull request

1. Делаем форк (fork) интересующего нас репозитория.
2. Делаем git clone для нашей версии этого репозитория. Так появляется версия на нашем аккаунте, и именно эту версию мы клонируем.
3. Создаём ветку с предлагаемыми изменениями.
4. Производим все изменения только в этой ветке.
5. Отправляем эти изменения на свой аккаунт (push).
6. В окне на GitHub появляется возможность отправить pull request.

## Команды используемые для работы в системе pull request

* Команда _**git clone**_ позволяет копировать или клонировать к себе репозитории из интернета. Для этого мы обращаемся к программе Git, указываем параметр clone ипосле этого даём адрес того репозитория, который надо скачать. Далее в папке, где вызывается команда git clone, появляется новая папка. И уже внутри этой папки будет лежать полная копия указанного нами репозитория.

* Команда _**git pull**_ позволяет скачать всё актуальное из нашего удалённого репозитория.
Команда очень простая. Мы указываем программу git и параметр pull. Она позволяет получить из интернета актуальное состояние удалённого репозитория и скачать его на наш репозиторий. 

>> > Обратите внимание, что pull — составная команда. Помимо выкачивания из интернета, она ещё и мержит, то есть сливает, изменения с нашими.
Если возникают какие-то конфликты, то окошко будет таким же, как при конфликтах обычного git merge. То есть коменда состоит из двух частей: первая часть скачивает изменения с удалённого репозитория, а вторая — сливает эти изменения с текущим репозиторием.

* Команда _**git push**_  позволяет отправить то, что есть на нашем репозитории, на удалённый репозиторий. Требует авторизации. Если у нет прав на внесение изменений в репозиторий, Git не позволит это делать. 

Абракадабра,,,,,,))))0
# Повторение

Для закрепления материала и проверки своих знаний предлагаем вам обращаться к указанным ресурсам:

[тренажер по git](https://learngitbranching.js.org/)

[![тренажер по git](data:image/jpeg;base64,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)](https://learngitbranching.js.org/)]

Заголовки языка маркдаун на гитхаб:

[![Заголовки маркдаун на гит хабе](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQZ7GZK0Y7xGQGQqWNS7YBAj_itHN-InG-32Q&usqp=CAU)](https://gist.github.com/Jekins/2bf2d0638163f1294637 )]
