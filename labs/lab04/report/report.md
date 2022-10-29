---
## Front matter
title: "Отчет по лабораторной работе №4"
subtitle: "Дисциплина: Архитектура компьютера"
author: "Дмитрий Юрьевич Дымченко"

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

Целью работы является освоение процедуры оформления отчетов с помощью легковесного языка разметки Markdown.


# Выполнение лабораторной работы


Для начала работы необходимо через терминал перейти в каталог курса и обновить локальный репозиторий командой git pull (рис. [-@fig:001]).

![Обновление репозитория.](image/1.png){ #fig:001 width=90% }

Для дальнейшей работы необходимо установить TeX Live, Pandoc и Pandoc-crossref. Сначала займемся установкой TeX Live (рис. [-@fig:002]), (рис. [-@fig:003]), (рис. [-@fig:004]).

![Начало установки TeX Live.](image/2.png){ #fig:002 width=90% }

![Завершение установки.](image/3.png){ #fig:003 width=90% }

![Добавление в PATH.](image/4.png){ #fig:004 width=90% }

Далее необходимо установить Pandoc и Pandoc Crossref (рис. [-@fig:005]), (рис. [-@fig:006]).

![Установка Pandoc 2.18](image/5.png){ #fig:005 width=90% }

![Установка Pandoc Crossref 0.3.13.0](image/6.png){ #fig:006 width=90% }

Затем распаковываем архивы и копируем файлы в нужный каталог. Командой ls проверяем успешность выполнения задачи (рис. [-@fig:007]).

![Распаковка архивов и перенос файлов.](image/7.png){ #fig:007 width=90% }

После установки необходимого ПО вернемся к выполнению работы. Проведем компиляцию шаблона с использованием Makefile. Далее проверим, создались ли файлы и удалим их командой make clean (рис. [-@fig:008]).

![Использование Makefile.](image/8.png){ #fig:008 width=90% }

# Выполнение заданий для самостоятельной работы

Заданием для самостоятельной работы было выполнение отчета к лабораторной работе №3 с использованием Markdown. Для этого необходимо оформить отчет, а затем командой make в каталоге отчета создать файлы .docx и .pdf (рис. [-@fig:009]), (рис. [-@fig:010]). 

![Компиляция шаблона лабораторной работы №3](image/9.png){ #fig:009 width=90% }

![Компиляция шаблона лабораторной работы №3](image/10.png){ #fig:010 width=90% }

# Выводы

В ходе выполнения данной работы я освоил процедуру оформления отчетов с помощью легковесного языка разметки Markdown.

