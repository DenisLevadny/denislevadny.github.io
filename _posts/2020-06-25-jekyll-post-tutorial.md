---
layout: post
title:  "Руководство с примерами по написанию постов на Jekyll markdown: kramdown"
author: Denis
categories: [ tutorial ]
tags: [ writing a post on Jekyll ]
image: assets/images/octojekyll.png
beforetoc: "Сюда можно подсматривать когда пишу новый пост, пока не запомню."
toc: true
---
Собираю здесь фрагменты кода и полезные ссылки для написания постов на языке markdown: kramdown. Вставляю только заголовки, примеры синтаксиса, иногда короткое описание.

#### Заголовки

```Заголовки
Заголовок первого уровня
========================
Заголовок второго уровня
-------------------------

#  Заголовок первого уровня
### Заголовок третьего уровня
###### Заголовок шестого уровня

#  Заголовок первого уровня #
### Заголовок третьего уровня ###
###### Заголовок шестого уровня ######
```

#### Цветной текст

orange
{: .color-orange}
yellow
{: .color-yellow}
green
{: .color-green}
teal
{: .color-teal}

orange text
{: .highlight-orange}


Это <span class="color-blue">blue</span> текст
<span class="color-green">green</span>
<span class="color-orange">orange</span>
<span class="color-indigo">indigo</span>
<span class="color-purple">purple</span>
<span class="color-pink">pink</span>
<span class="color-yellow">yellow</span>
<span class="color-teal">teal</span>
<span class="color-cyan">cyan</span>
<span class="color-red">red</span><br>

<span class="highlight-teal">teal</span>
<span class="highlight-green">green</span>
<span class="highlight-orange">orange</span>
<span class="highlight-red">red</span>
<span class="highlight-black">black</span>
<span class="highlight-yellow">yellow</span>

```текст
<span class="color-blue">Some</span>
<span class="color-green">cool</span>
<span class="color-orange">colorful</span>
<span class="color-red">text.</span><br>
```

```фон
<span class="highlight-teal">teal</span>
<span class="highlight-green">green</span>
<span class="highlight-orange">orange</span>
<span class="highlight-red">red</span>
<span class="highlight-black">black</span>
<span class="highlight-yellow">yellow</span>
```


#### Цитаты

```Цитаты
> Первый уровень цитирования
>> Второй уровень цитирования
>>> Третий уровень цитирования
>
>Первый уровень цитирования
```

#### Списки

```Списки
* Проводник
+ Полупроводник
- Диэлектрик
```

```Списки
1. Проводник
2. Полупроводник
3. Диэлектрик
```

#### Горизонтальные

```Горизонтальные
Первая часть текста, который необходимо разделить
***
Вторая часть текста, который необходимо разделить
```

```Горизонтальные
Первая часть текста, который необходимо разделить

-- -- -  -- --- 

Вторая часть текста, который необходимо разделить
```

#### Ссылки

```Ссылки
[название](http://example.com/ "Необязательная подсказка при наведении")
```

```Ссылки
<http://example.com/>
```

В результате на экран выводится следующее: <http://example.com/>

```Ссылки
<address@example.com>
```

Локальные сноски по id

```Ссылки
[название] [id]:
```

В этом случае возможно определить идентификатор в любом месте документа

```Ссылки
[id]: http://example.com/ "Необязательная подсказка"
```

#### Выделение

```Выделение
*курсив*
_курсив_
```

```Выделение
**полужирный**
__полужирный__
```

```Выделение
***полужирный курсив***
___полужирный курсив___
```

#### Изображения

```Изображения
![Альтернативный текст](/путь/к/изображению.jpg "Необязательная подсказка")
```

```Изображения
![Альтернативный текст][id]
```

```Изображения
[id]: путь/к/изображению "Необязательная подсказка"
```

Квадратные скобки, в которых указывается альтернативный изображению текст (он станет содержимым атрибута в элементе img)

Markdown не позволяет задать размеры изображения (ширину, высоту)

### Обратный слеш

Может употребляться в Markdown перед специальными символами для того, чтобы они воспринимались в их буквальном (а не служебном) значении.


![octojekyll](/assets/images/octojekyll1.png "octojekyll")
