---
## Front matter
title: "Отчет по лабораторной работе №7"
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

Научиться строить различные графики, работать с комплексными числами и специальными функциями.

# Задание

Построить параметрический график, график в полярных координатах, график неявной функции, график в комплексной плоскости, график специальной функции.

# Выполнение лабораторной работы

## Шаг 1

Включила журналирование. Построила график трех периодов циклоиды радиуса 2. Соответствующие команды показаны на Рисунке 1 (рис - @fig:001).

![Три периода циклоиды](images/1.png){#fig:001 width=70%}

## Шаг 2

Построила улитку Паскаля в декартовых координатах (команды показаны на Рисунке 2 (рис - @fig:002), график на Рисунке 3 (рис - @fig:003)) и полярных координатах (команды показаны на Рисунке 4 (рис - @fig:004), график на Рисунке 3 (рис - @fig:005)).

![Построение улитки Паскаля в декартовых координатах](images/2.png){#fig:002 width=70%}

![График улитки Паскаля в декартовых координатах](images/limacon.png){#fig:003 width=70%}

![Построение улитки Паскаля в полярных координатах](images/3.png){#fig:004 width=70%}

![График улитки Паскаля в полярных координатах](images/limacon_polar.png){#fig:005 width=70%}

## Шаг 3

Построила график неявной функции с помощью команды ezplot (рис - @fig:006 и - @fig:007).

![Построение графика неявной функции](images/4.png){#fig:006 width=70%}

![График неявной функции](images/impl1.png){#fig:007 width=70%}

Также использовала неявную функцию для построения круга и касательной к нему (рис - @fig:008 и - @fig:009).

![Построение графика касательной к кругу](images/5.png){#fig:008 width=70%}

![График касательной к окружности](images/impl2.png){#fig:009 width=70%}

## Шаг 4

Произвела основные арифметические операции с двумя комплексными числами и построила графики в комплексной плоскости с помощью команды compass (рис - @fig:010). График представлен на Рисунке 11 (рис - @fig:011).

![Операции с комплексными числами и построение графика на комплексной плоскости](images/6.png){#fig:010 width=70%}

![График в комплексной плоскости](images/complex.png){#fig:011 width=70%}

## Шаг 5

Построила графики функций $Г(x+1) и n!$ на одном графике (рис - @fig:012 и рис - @fig:013).

![Построение функции гамма и факториала на одном графике](images/8.png){#fig:012 width=70%}

![График функции гамма и факториала](images/gamma.png){#fig:013 width=70%}

Вертикальные асимптоты на графике в районе отрицательных чисел не являются истинными частями графика - это артефакты вычисления. Чтобы избавиться от них, разделила область значений на отдельные интервалы (рис - @fig:014). Получившийся график представлен на Рисунке 15 (рис - @fig:015).

![Построение функции гамма и факториала с разбиением на интервалы](images/9.png){#fig:014 width=70%}

![График функции гамма и факториала без артефактов](images/gamma2.png){#fig:015 width=70%}

# Выводы

Я научилась строить параметрический график, график в полярных координатах, график неявной функции, график в комплексной плоскости, график специальной функции с помощью Octave. Результаты работы находятся в [репозитории на GitHub](https://github.com/ZlataDyachenko), а также есть [скринкаст выполнения лабораторной работы](https://www.youtube.com/watch?v=-cnIgjUwAmc).
