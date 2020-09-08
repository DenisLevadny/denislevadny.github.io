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


Это <span class="color-blue">синий</span> текст
<span class="color-green">зеленый</span>
<span class="color-orange">оранжевый</span>
<span class="color-indigo">оранжевый</span>
<span class="color-purple">оранжевый</span>
<span class="color-pink">оранжевый</span>
<span class="color-yellow">оранжевый</span>
<span class="color-teal">оранжевый</span>
<span class="color-cyan">оранжевый</span>
<span class="color-red">красный</span><br>

<span class="highlight-orange">And</span>
<span class="highlight-green">some</span>
<span class="highlight-yellow">highlighting</span>
<span class="highlight-teal">styles.</span>
<span class="highlight-red">styles.</span>

```текст
<span class="color-blue">Some</span>
<span class="color-green">cool</span>
<span class="color-orange">colorful</span>
<span class="color-red">text.</span><br>
```

```фон
<span class="highlight-blue">And</span>
<span class="highlight-green">some</span>
<span class="highlight-orange">highlighting</span>
<span class="highlight-red">styles.</span>
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
