---
## Front matter
title: "Отчет по лабораторной работе №4"
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

Научиться решать системы линейных уравнений с помощью Octave.

# Задание

Решить систему уравнений методом Гаусса, с использованием левого деления и с помощью LU-разложения и LUP-разложения.

# Выполнение лабораторной работы

## Шаг 1

Построила расширенную матрицу системы линейных уравнений. Для явного решения методом Гаусса сначала добавила к третьей строке первую строку, умноженную на −1. Далее добавила к третьей строке вторую строку, умноженную на −1.5. Из полученной треугольной матрицы, представленной на Рисунке 1 (рис - @fig:001), как и выполненные для ее получения команды, можно получить решение.

![Метод Гаусса](images/1_1.png){#fig:001 width=70%}

Для непосредственного поиска треугольной формы матрицы использовала встроенную функцию. Из результата ее выполнения, представленного на Рисунке 2 (рис - @fig:002), решение системы очевидно. На Рисунке 2 (рис - @fig:002) также показано представление большего числа десятичных разрядов чисел.

![Поиск треугольной формы и изменение формата вывода чисел](images/1_2.png){#fig:002 width=70%}

## Шаг 2

Для решения системы вида $Ax=b$ использовала встроенную операцию левого деления, что продемонстрированно на Рисунке 3 (рис - @fig:003).

![Левое деление](images/2.png){#fig:003 width=70%}

## Шаг 3

С помощью Octave расписала LU-разложение данной матрицы в файле *lu_my2.m*, содержание которого показано на Рисунке 4 (рис - @fig:004). Запуск файла и результат выполнения показан на Рисунке 5 (рис - @fig:005).

![LU-разложение](images/3_1.png){#fig:004 width=70%}

![LU-разложение](images/3_2.png){#fig:005 width=70%}

## Шаг 4

На Рисунке 6 (рис - @fig:006) показано вычисление LUP-разложения матрицы с помощью встроенной функции.

![LUP-разложение матрицы](images/4.png){#fig:006 width=70%}

# Выводы

Я ознакомилась с решением систем линейных уравнений в Octave, а именно использованием метода Гаусса, левого деления, LU-разложения и LUP-разложения. Результаты работы находятся в [репозитории на GitHub](https://github.com/ZlataDyachenko), а также есть [скринкаст выполнения лабораторной работы](https://www.youtube.com/watch?v=4PyG0GBOLMg).
