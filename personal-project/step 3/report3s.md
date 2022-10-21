---
# Front matter
title: "Отчет по выполнению 3 этапа индивидуального проекта"
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

Добавить к сайту достижения.

# Задание

- Добавить информацию о навыках (Skills).
- Добавить информацию об опыте (Experience).
- Добавить информацию о достижениях (Accomplishments).
- Сделать пост по прошедшей неделе.
- Добавить пост на тему по выбору:
    * Легковесные языки разметки.
    * Языки разметки. LaTeX.
    * Язык разметки Markdown.


# Выполнение третьего этапа проекта

## Шаг 1

Для добавления информации о навыках изменила соответствующие разделы файла */blog/blog/content/home/skills.md*, показанный на Рисунке 1 (рис. -@fig:001). Вид данного раздела на сайте представлен на Рисунке 2 (рис. -@fig:002).

![Добавление навыков](images/2.png){#fig:001 width=70%}

![Вид раздела сайта с навыками](images/6.png){#fig:002 width=70%}

## Шаг 2

Для добавления информации об опыте изменила файл */blog/blog/content/home/experience.md*, содержание которого представлено на Рисунке 3 (рис. -@fig:003). Вид данного раздела на сайте представлен на Рисунке 4 (рис. -@fig:004).

![Добавление информации об опыте](images/1.png){#fig:003 width=70%}

![Вид раздела сайта об опыте](images/7.png){#fig:004 width=70%}

## Шаг 3

Для добавления информации о достижениях изменила файл */blog/blog/content/home/accomplishments.md*, содержание которого представлено на Рисунке 5 (рис. -@fig:005). Вид данного раздела на сайте представлен на Рисунке 6 (рис. -@fig:006).

![Добавление информации о достижениях](images/3.png){#fig:005 width=70%}

![Вид раздела сайта о достижениях](images/8.png){#fig:006 width=70%}

## Шаг 4

Для создания поста о прошедшей неделе создала папку *blog/blog/content/post/week2*, а в ней файл *index.md*. Кроме того, добавила в папку сопровождающую картинку. Часть файла *blog/blog/content/post/week2/index.md* представлена на Рисунке 7 (рис. -@fig:007). Внешний вид части поста на сайте представлен на Рисунке 8 (рис. -@fig:008).

![Создание поста о прошедшей неделе](images/5.png){#fig:007 width=70%}

![Пост о прошедшей неделе на сайте](images/9.png){#fig:008 width=70%}

## Шаг 5

Для создания поста на тему "Легковесные языки разметки" создала папку *blog/blog/content/post/lang*, а в ней файл *index.md*. Кроме того, добавила в папку сопровождающую картинку. Содержание файла *blog/blog/content/post/lang/index.md* представлено на Рисунке 9 (рис. -@fig:009). Внешний вид части поста на сайте представлен на Рисунке 10 (рис. -@fig:010).

![Создание поста на тему "Легковесные языки разметки"](images/4.png){#fig:009 width=70%}

![Пост на сайте](images/10.png){#fig:010 width=70%}


# Выводы

Я добавила на сайт информацию о достижениях, навыках, опыте, а также написала два новых поста. Результаты работы видны [на сайте](https://zlatadyachenko.github.io/), а также есть [скринкаст выполнения лабораторной работы](https://www.youtube.com/watch?v=GjxcETtTWzc).
