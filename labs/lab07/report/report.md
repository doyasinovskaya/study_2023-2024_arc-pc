---
## Front matter
title: "Отчёт по лабораторной работе №7"
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

Целью лабораторной работы является освоение процедуры компиляции и сборки программ, написанных на ассемблере NASM.


# Выполнение лабораторной работы

Создаю каталог для лабораторной работы №7, перешла в него и создала файл.

![Создание каталога и файла](/home/daryayasinovskaya/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab07/report/image/Снимок экрана от 2023-11-19 11-18-00.png){#fig:001 width=80%}

Ввожу в файл lab7-1.asm текст программы из листинга 7.1

![Файл с текстом](/home/daryayasinovskaya/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab07/report/image/Снимок экрана от 2023-11-19 11-22-53.png){#fig:002 width=80%}

Создаю исполняемый файл и запускаю его.

![Запуск файла](/home/daryayasinovskaya/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab07/report/image/Снимок экрана от 2023-11-19 11-26-07.png){#fig:003 width=80%}

Добавляю инструкции в соотвестсвии с листингом 7.2

![Изменение файла](/home/daryayasinovskaya/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab07/report/image/Снимок экрана от 2023-11-19 12-11-51.png){#fig:005 width=80%}

Создаю исполняемый файл и запускаю его.

![Запуск файла](/home/daryayasinovskaya/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab07/report/image/Снимок экрана от 2023-11-19 12-02-31.png){#fig:004 width=80%}

Изменяю текст программы, чтобы он выводил сначала сообщение №3, затем сообщение №2, а затем сообщение №1

![Изменение текста](/home/daryayasinovskaya/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab07/report/image/Снимок экрана от 2023-11-19 12-12-46.png){#fig:007 width=80%}

Создаю исполняемый файл и запускаю его.

![Запуск файла](/home/daryayasinovskaya/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab07/report/image/Снимок экрана от 2023-11-19 12-13-19.png){#fig:006 width=80%}
  
Создаю файл lab7-2.asm и ввожу в него текст из листинга 7.3

![Ввод текста](/home/daryayasinovskaya/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab07/report/image/Снимок экрана от 2023-11-19 12-18-20.png){#fig:006 width=80%} 

Создаю исполняемый файл и проверяю его работу для разных значений.

![Вывод программы для разных значение В](/home/daryayasinovskaya/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab07/report/image/Снимок экрана от 2023-11-19 12-33-38.png){#fig:006 width=80%} 

Создаю файл листинга для программы из файла lab7-2.asm

![Файл листинга](/home/daryayasinovskaya/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab07/report/image/Снимок экрана от 2023-11-19 12-35-11.png){#fig:006 width=80%} 

Открываю файл листинга с помощью текстового редактора mcedit.

![Открытие файла](/home/daryayasinovskaya/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab07/report/image/Снимок экрана от 2023-11-19 12-35-31.png){#fig:006 width=80%} 


Удаляю один операнд из строчки с двумя операндами. Теперь программа выдает ошибку (error: invalid combination of opcode and operands)

![Файл с ошибкой](/home/daryayasinovskaya/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab07/report/image/Снимок экрана от 2023-11-25 21-18-59.png){#fig:006 width=80%} 

### Самостоятельная работа

Написала программу для нахождения наибольшей из 3 целочисленных переменных

![Программа](/home/daryayasinovskaya/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab07/report/image/Снимок экрана от 2023-11-25 23-33-07.png){#fig:006 width=80%}

Создаю исполняемый файл и проверяю программу

![Запуск файла](/home/daryayasinovskaya/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab07/report/image/Снимок экрана от 2023-11-25 21-43-38.png){#fig:006 width=80%}

Написала программу, которая для введенных с клавиатуры значений х и а вычисляет
значение заданной функции f(x) и выводит результат вычислений.
 
![Программа](/home/daryayasinovskaya/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab07/report/image/Снимок экрана от 2023-11-25 23-32-49.png){#fig:006 width=80%} 

Создаю исполняемый файл и проверяю программу

![Запуск файла](/home/daryayasinovskaya/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab07/report/image/Снимок экрана от 2023-11-25 23-32-30.png){#fig:006 width=80%} 

### Выводы

Я освоила процедуры компиляции и сборки программ, написанных на ассемблере NASM.

::: {#refs}
:::
