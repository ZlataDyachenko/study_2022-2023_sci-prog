---
# Front matter
title: "Отчет по выполнению 2 этапа индивидуального проекта"
subtitle: "Дисциплина: Научное программирование"
author: "Выполнила Дяченко Злата Константиновна, НПМмд-02-22"

# Generic otions
lang: ru-RU
toc-title: "Содержание"

# Bibliography

# Pdf output format
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n
polyglossia-lang:
  name: russian
  options:
  - spelling=modern
  - babelshorthands=true
polyglossia-otherlangs:
  name: english
### Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Misc options
indent: true
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Добавить к сайту данные о себе.

# Задание

—  Разместить фотографию владельца сайта.   
—  Разместить краткое описание владельца сайта (Biography).   
—  Добавить информацию об интересах (Interests).   
—  Добавить информацию от образовании (Education).  
—  Сделать пост по прошедшей неделе.  
—  Добавить пост на тему по выбору:   
    Управление версиями. Git.   
    Непрерывная интеграция и непрерывное развертывание (CI/CD).   


# Выполнение второго этапа проекта

## Шаг 1

Для размещения фотографии владельца сайта изменила находящийся в шаблоне снимок на свой *blog/blog/content/authors/admin/avatar.jpg*,что показано на Рисунке 1 (рис. -@fig:001).

![Установка фотографии](images/5.png){#fig:001 width=70%}

## Шаг 2

Для размещения на сайте информации о владельце, об его интересах и образовании изменила соответствующие разделы файла */blog/blog/content/authors/admin/_index.md*, показанный на Рисунке 2 (рис. -@fig:002).

![Изменение информации о владельце в файле content/authors/admin/_index.md](images/1.png){#fig:002 width=70%}

Кроме того, разместила ссылки на социальные сети, а именно на сайте имеется кнопка для быстрого перехода к разделу contact, кнопка для перехода на мою станицу на GitHub и для перехода в мой профиль в социальной сети "ВКонтакте" (рис. -@fig:003).

![Добавление ссылок на социальные сети в файле content/authors/admin/_index.md](images/2.png){#fig:003 width=70%}

На Рисунке 4 (рис. -@fig:004) представлено описание владельца сайта. Вид всех этих разделов на сайте представлен на Рисунке 5 (рис. -@fig:005).

![Описание владельца сайта в файле content/authors/admin/_index.md](images/3.png){#fig:004 width=70%}

![Вид раздела сайта, посвященного владельцу](images/11.png){#fig:005 width=70%}

## Шаг 3

Сделала пост о прошедшей неделе, отредактировав файл *blog/blog/content/post/getting-started/index.md*. Начало файла представлено на Рисунке 6 (рис. -@fig:006). Размещенную по пути *blog/blog/content/post/getting-started/featured.jpg* изменила на подходящую к посту. Вид на сайте начала получившегося поста представлен на Рисунке 7 (рис. -@fig:007). Ознакомиться с содержанием поста можно на самом сайте.

![Создание поста о прошедшей неделе](images/6.png){#fig:006 width=70%}

![Пост о прошедшей неделе на сайте](images/10.png){#fig:007 width=70%}

## Шаг 4

Для создания поста на тему "Управление версиями. Git." отредактировала файл *blog/blog/content/post/writing-technical-content/index.md*. Начало файла представлено на Рисунке 8 (рис. -@fig:008).

![Создание поста на тему "Управление версиями. Git."](images/7.png){#fig:008 width=70%}

При описании основных команд в посте использовала блоки кода, а также добавляла перед каждым блоком символ терминала с помощью строк, показанных на Рисунке 9 (рис. -@fig:009).

![Выделение терминов жирным шрифтом, создание блоков кода и добавление значков перед ними](images/8.png){#fig:009 width=70%}

Внешний вид данной части поста на сайте представлен на Рисунке 10 (рис. -@fig:010). Прикрепленное к посту изображение также было изменено, с чем можно ознакомиться на сайте.

![Пост на сайте](images/9.png){#fig:010 width=70%}

# Выводы

Я добавила на сайт информацию о себе (фото, описание, ссылки на социальные сети, данные об образовании, интересы). Результаты работы видны [на сайте](https://zlatadyachenko.github.io/), а также есть [скринкаст выполнения лабораторной работы](https://www.youtube.com/watch?v=oQyg6NSQ6vg).
