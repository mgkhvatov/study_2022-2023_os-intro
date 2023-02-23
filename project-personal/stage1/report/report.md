---
## Front matter
title: "Индивидуальный проект."
subtitle: "Этап 1"
author: "Хватов Максим Григнорьевич"

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

* Установить необходимое программное обеспечение.
* Скачать шаблон темы сайта.
* Разместить его на хостинге git.
* Установить параметр для URLs сайта.
* Разместить заготовку сайта на Github pages.

# Теоретическое введение

Hugo — один из самых популярных генераторов статических сайтов с открытым исходным кодом. Hugo обладает большой скоростью и хорошей гибкостью при разработке на нём.

Мы можем использовать различные тем для того, чтобы сразу стилизовать нашу страницу для дальнейшего выкладывания ее в интернет. Также, можно отметить, ч то сайты, сгенерированные с помощью генераторов имеют лучшую SEO-оптимизацию.

И так как, сайт у нас генерируется статически, то он является сгенерированным на стороне клиента.

# Выполнение лабораторной работы

* Скачаем Hugo, и установим его с помощью команды `snap install hugo go`
* После этого создадим пустой репозиторий на гитхабе
* Клонируем репозиторий себе на компьютер `git clone git@github.com:mgkhvatov/blog.git`
* Создаем еще один репозиторий с на сонове темплейта Wowchemy названием mgkhvatov.github.io
* Клолнируем предыдущий репозиторий и связываем с ним папку public, которая была сгенерирована с помощью команды `hugo` в дериктории с репозиторием blog/
* Привязываем public при помощи команды `git submodule add git@github.com:mgkhvatov/blog.git public`
* Заново генерируем папку public при помощи команды `hugo`
* Переходим в нее и выполняем команды для коммита и отправки изменений в гитхаб `git commit -am "Generated public"` -> `git push origin main`
* После этого вводим название второго репозипория в строку браузера и получаем на выходе готовый рабочий сайт.

# Выводыё

Я научился настраивать репозиторий гитхаба для деплоя на нём проекта, собранного с помощью генератора статических сайтов Hugo.
А также научился генерировать этот самый статический сайт с помощью команд, встроенных в Hugo.
