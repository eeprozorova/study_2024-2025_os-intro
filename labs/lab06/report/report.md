---
## Front matter
title: "Лабораторная работа №6"
subtitle: "Основы интерфейса взаимодействия пользователя с системой Unix на уровне командной строки"
author: "Прозорова Елизавета Евгеньевна"

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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Приобретение практических навыков взаимодействия пользователя с системой посредством командной строки.

# Выполнение лабораторной работы

1. Я определила имя домашнего каталога через Thunar. 

![Домашний каталог](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/2025-03-18_20-37-52.png){#fig:001 width=70%}

2. Я перешла в каталог /tmp/ и вывела его содержимое с помощью ls. с различными опциями.

![Содержимое каталога tmp](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/2025-03-18_20-39-47.png){#fig:002 width=70%}

Затем я перешла в каталог /var/spool чтобы посмотреть есть ли там подкаталог с именем cron. Он есть.

![Каталог var/spool с подкаталогом cron](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/2025-03-18_22-05-41.png){#fig:003 width=70%}

3. В домашнем каталоге создала новый каталог с именем newdir, в котором создала новый каталог с именем morefun.

![Каталог newdir и morefun](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/2025-03-18_22-09-03.png){#fig:004 width=70%}

В домашнем каталоге создала одной командой три новых каталога с именами letters, memos, misk. Затем удалила эти каталоги одной командой.

![Каталоги с именами letters, memos, misk](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/2025-03-18_22-10-30.png){#fig:005 width=70%}

Затем я попробовала удалить newdir командой rm, у меня не получилось. Тогда я попробовала rmdir, тоже не получилось. После этого я использовала команду rm -r, она сработала.

![Удаление newdir](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/2025-03-18_22-11-46.png){#fig:006 width=70%}

4. Теперь я ввела команду man.

![Команда man](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/2025-03-18_22-12-33.png){#fig:007 width=70%}

Команда man на ls. 

![Внутренности ls](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/2025-03-18_22-13-23.png){#fig:008 width=70%}

Я определила опцию команды ls, которую нужно использовать для просмотра содержимое не только указанного каталога, но и подкаталогов, входящих в него.

![Опция ls](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/2025-03-18_22-14-21.png){#fig:009 width=70%}

5. Затем я определила набор опций команды ls, позволяющий отсортировать по времени последнего изменения выводимый список содержимого каталога с развёрнутым описанием файлов.

![Опция команды ls для сортировки содержимого каталога по времени](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/2025-03-18_22-15-06.png){#fig:010 width=70%}

6. Я использовала команду man для просмотра описания команды cd.

![Описание cd](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/2025-03-18_22-17-06.png)){#fig:011 width=70%}

Просмотр описания команды pwd.

![Описание pwd](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/2025-03-18_22-17-54.png){#fig:012 width=70%}

Просмотр описания команды mkdir.

![Описание mkdir](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/2025-03-18_22-18-26.png){#fig:013 width=70%}

Просмотр описания команды rm.

![Описание rm](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/2025-03-18_22-18-59.png){#fig:014 width=70%}

7. Затем я посмотрела что делает команда history.

![History](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab06/report/image/2025-03-18_22-19-46.png){#fig:015 width=70%}

# Выводы

В ходе работы я приобрела навыки работы с системой посредством командной строки.

::: {#refs}
:::
