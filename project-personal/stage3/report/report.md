---
## Front matter
title: "Отчёт по индивидуальному проекту"
subtitle: "Этап 3"
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

Научиться работать с блоками информации на сайте через конструктор Hugo

# Задание

Добавить к сайту достижения.

1. Список достижений.
2. Добавить информацию о навыках (Skills).
3. Добавить информацию об опыте (Experience).
4. Добавить информацию о достижениях (Accomplishments).
5. Сделать пост по прошедшей неделе.
6. Сделать пост на тему: Легковесные языки разметки.


# Теоретическое введение

Файлы для изменения информации о себе согласно заданиям лежат в папке content/_index.md.
Чтобы изменить информацию нужно найти блоки согласно заданию.

# Выполнение лабораторной работы

Находим блок skills и меняем информацию под себя, можно также изменить значки на каждый скилл.

![Skills](image/skills.png){#fig:001 width=70%}

далее находим блок experience и меняем также под себя, описывая свой опыт и то, с чем приходилось работать.

![experience](image/experience.png){#fig:001 width=70%}

находим блок accomplishments и меняем под себя

![accomplishments](image/accomplishments.png){#fig:001 width=70%}

пишем пост о прошедшей неделе и пост на тему Легковесных языков разметки.

![accomplishments](image/posts.png){#fig:001 width=70%}

# Выводы

Я научился работать с блоками информации о себе и изменять её через конструктор Hugo.

# Список литературы{.unnumbered}

::: {#refs}
:::
