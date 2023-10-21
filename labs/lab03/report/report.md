---
## Front matter
title: "Отчёт по лабораторной работе №3"
subtitle: "дисциплина: Архитектура компьютеров"
author: "Ясиновская Дарья Олеговна"

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
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Освоить процедуры оформления отчетов с помощью легковесного
языка разметки Markdown.


# Выполнение лабораторной работы

Открыла терминал и перешла в каталог курса, затем обновила локальный репозиторий с помощью команды git pull

![Обновление репозитория](image/рис 1.png){#fig:001 width=80%}

Перешла в каталог с шаблоном отчета по лабораторной работе №3 

![Каталог с шаблоном отчета](image/рис 2.png){#fig:002 width=80%}

Провела компиляцию шаблона с помощью команды make

![Компиляция шаблона](image/рис 3.png){#fig:003 width=80%}

Убедилась в наличии файлов 

![Папка с файлами](image/рис 4.png){#fig:004 width=80%}

Удалила полученные файлы с помощью команды make clean

![Удаление файлов](image/рис 5.png){#fig:005 width=80%}

Убедилась, что файлы удалены

![Проверка удаления файлов](image/рис 6.png){#fig:006 width=80%}

Открыла файл report.md с помощью текстового редактора gedit

![Открытие файла с помощью текстового редактора gedit](image/рис 7.png){#fig:007 width=80%}

Изучила структуру файла

![Структура файла](image/рис 8.png){#fig:008 width=80%}



# Выводы

Я освоила процедуры оформления отчетов с помощью легковесного
языка разметки Markdown.

# Список литературы{.unnumbered}

::: {#refs}
:::
