---
## Front matter
title: "Отчёт по индивидуальному проекту"
subtitle: "Этап 6"
author: "Хватов Максим Григорьевич"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
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
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Научиться добавлять информацию о своих проектах на сайт, собранном через Hugo

# Задание

1. Сделать записи для персональных проектов.
2. Сделать пост по прошедшей неделе.
3. Добавить пост на тему *Языки научного программирования.*

# Теоретическое введение

Нужные файлы лежат в директории content/projects и content/post

# Выполнение лабораторной работы

Создаю две папки по своим проектам в директории content/projects. Добавляю туда необходимую информацию и фото.

![Проекты](image/projs.png){#fig:001 width=70%}

Создаю пост о прошедшей недел, копируя предыдущий, т.к. все однообразно. Пишу пост на тему *Научных языков программирования*. Все манипуляции провожу в папке, соответствующей посут в директории content/post

![Посты](image/posts.png){#fig:001 width=70%}

# Выводы

Я научился добавлять информацию о проектах на сайт, используя Hugo.

# Список литературы{.unnumbered}

::: {#refs}
:::
