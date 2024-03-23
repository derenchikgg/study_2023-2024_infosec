---
## Front matter
title: "Лабораторная работа 4"
subtitle: "Дискреционное разграничение прав в Linux. Расширенные атрибуты"
author: "Панченко Денис Дмитриевич"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: false # List of figures
lot: false # List of tables
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

Получение практических навыков работы в консоли с расширенными атрибутами файлов.

# Задание

Получить практические навыки работы в консоли с расширенными атрибутами файлов.

# Выполнение лабораторной работы

От имени пользователя guest определите расширенные атрибуты файла (рис. 1).

![Атрибуты](image/1.png){#fig:001 width=70%}

Установим на файл права, разрешающие чтение и запись для владельца файла (рис. 2).

![Права](image/2.png){#fig:002 width=70%}

Попробуем установить на файл расширенный атрибут a от имени пользователя guest (рис. 3).
Не вышло.

![Атрибут а](image/3.png){#fig:003 width=70%}

Зайдем в другую консоль с правами администратора и попробуем установить расширенный атрибут a на файл (рис. 4).

![Атрибут а](image/4.png){#fig:004 width=70%}

От пользователя guest проверим правильность установления атрибута (рис. 5).

![Проверка](image/5.png){#fig:005 width=70%}

Выполним дозапись в файл слова «test» и выполним чтение файла (рис. 6).

![Дозапись](image/6.png){#fig:006 width=70%}

Попробуем удалить файл (рис. 7).
Удалить файл не вышло.

![Удаление](image/7.png){#fig:007 width=70%}

Попробуем установить на файл права, запрещающие чтение и запись для владельца файла (рис. 8).
Не получилось.

![Установка прав](image/8.png){#fig:008 width=70%}

Снимем расширенный атрибут a с файла от имени суперпользователя (рис. 9).

![Снятие атрибута](image/9.png){#fig:009 width=70%}

Повторим операции, которые нам ранее не удавалось выполнить (рис. 10).

![guest](image/10.png){#fig:010 width=70%}

Повторим наши действия по шагам, заменив атрибут «a» атрибутом «i» (рис. 11 - 12).
Выполнение команд с атрибутом "i" не отличается от выполнения команд с атрибутом "a".

![Повтор действий](image/11.png){#fig:011 width=70%}

![Повтор действий](image/12.png){#fig:012 width=70%}

# Вывод

В результате выполнения работы я повысили свои навыки использования интерфейса командой строки, познакомился на примерах с тем, как используются основные и расширенные атрибуты при разграничении доступа. Имел возможность связать теорию дискреционного разделения доступа (дискреционная политика безопасности) с её реализацией на практике в ОС Linux. Опробовал действие на практике расширенных атрибутов «а» и «i».
