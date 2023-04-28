---
## Front matter
title: "Отчёт по индвидуальному проекту"
subtitle: "Этап 4"
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

Научиться редактировать содержимое сайта, разрабатываемого на Hugo.

# Задание

Добавить к сайту ссылки на научные и библиометрические ресурсы.

1. Зарегистрироваться на соответствующих ресурсах и разместить на них ссылки на сайте:
    * eLibrary : https://elibrary.ru/;
    * Google Scholar : https://scholar.google.com/;
    * ORCID : https://orcid.org/;
    * Mendeley : https://www.mendeley.com/;
    * ResearchGate : https://www.researchgate.net/;
    * Academia.edu : https://www.academia.edu/;
    * arXiv : https://arxiv.org/;
    * github : https://github.com/.
2. Сделать пост по прошедшей неделе.
3. Добавить пост на тему "Работа с библиографией."


# Теоретическое введение

Вся теория была описана в прошлых отчётах, а узнать более подробно про генерацию статических сайтов можно на официальной странице Hugo.

# Выполнение лабораторной работы

Запускаем сервер с помощью команды `hugo server`

Заходим в каталог content/authors/admin/_index.md и находим блок с информацией о внешних ссылках на дополнительные ресурсы. 
Меняем эти ссылки на ссылки своих профилей.

![Задание 1](image/1.png){#fig:001 width=70%}

Заходим в каталог content/posts и создаём две папки для постов. Одна папка - для прошедшей недели, а другая для статьи на выбор.

![Задание 2](image/2.png){#fig:001 width=70%}
![Задание 3](image/3.png){#fig:001 width=70%}

Останавливаем сервер и собираем сайт с помощью команды `hugo`. Отправляем изменения на github командой `git push origin main`, предварительно зафиксировав изменения в файлах.


# Выводы

Я научился редактировать содержимое сайта на Hugo.

# Список литературы{.unnumbered}

::: {#refs}
:::
