---
## Front matter
title: "Лабораторная работа №7"
subtitle: "Анализ файловой системы Linux. Команды для работы с файлами и каталогами"
author: "Елизавета Евгеньевна Прозорова"

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

Ознакомление с файловой системой Linux, её структурой, именами и содержанием каталогов. Приобретение практических навыков по применению команд для работы с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы

# Выполнение лабораторной работы

1. Я начала с того что выполнила все примеры, приведённые в первой части описания лабораторной работы.

1.1. Я выполнила команды на копирование файлов и каталогов.

![Копирование файлов и каталогов](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_18-51-49.png){#fig:001 width=70%}

1.2. Я выполнила команды на перемещение и переименование файлов и каталогов.

![Перемещение файлов и каталогов](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_18-49-56.png){#fig:002 width=70%}

1.3. Я выполнила команды на изменение прав доступ. Я создала файл с правом выполнения для владельца, затем лишила этот файл этого права.

![Права доступа файла may](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_19-26-45.png){#fig:003 width=70%}

Я создала каталог monthly с запретом на чтение для членов группы и всех остальных пользователей:

![mouthly](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_19-27-17.png){#fig:004 width=70%}

Я создала файл ~/abc1 с правом записи для членов группы.

![abc1](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_19-27-47.png){#fig:005 width=70%}

1.4. Я выполнила команды на анализ файловой системы. Сначало я попробовала команду mount.

![mount](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_19-29-57.png){#fig:006 width=70%}

Затем я ввела команду для просмотра файла /etc/fstab. 

![Команда cat](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_19-31-45.png){#fig:007 width=70%}

Команда для определения объёма свободного пространства на файловой системе. 

![Команда df](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_19-32-35.png){#fig:008 width=70%}

Команда для проверки (а в ряде случаев восстановления) целостности файловой системы:

![fsck](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_19-33-51.png){#fig:009 width=70%}

2. Я выполнила следующие команды.

Я  скопировала файл /usr/include/sys/io.h в домашний каталог. Создала каталог ski.plases и переместила файл equipment в ski.plases

![Перемещение файла equipment в ski.plases](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_20-38-35.png){#fig:010 width=70%}

Переименовала файла equipment в equiplist

![Переименование файла equipment в equiplist](//home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_20-38-52.png)){#fig:011 width=70%}

Создала файла abc1 и скопировала его в ski.plases как equiplist2

![Файл abc1](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_20-42-06.png){#fig:012 width=70%}

Создала каталога equipment в ski.plases и переместила equiplist и equiplist2 в каталог equipment

![Каталог equipment](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_20-43-53.png){#fig:013 width=70%}

Затем я создала и перемеместила каталога newdir в ski.plases с новым именем plans

![Новый каталог plans](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_20-44-51.png){#fig:014 width=70%}

3. Теперь я  присвоила перечисленным файлам права доступа (файлы создала заранее)

![Присвоение прав доступа](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_21-24-32.png){#fig:015 width=70%}

4. Я просмотрела содержимое файла /etc/passwd

![Использование команды cat](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_21-26-10.png){#fig:016 width=70%}

Я скопировала файл ~/feathers в файл ~/file.old.

![Копирование feathers в file.old](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_21-54-16.png){#fig:017 width=70%}

Переместила файл ~/file.old в каталог ~/play, скопировала каталог ~/play в каталог ~/fun и переместила каталог ~/fun в каталог ~/play и назвала его games.

![Работа с каталогом play](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_21-57-49.png){#fig:018 width=70%}

Я лишила себя права на чтение файла ~/feathers и попробовала несколько команд на проверку. Когда я убедилась, я вернула права.

![Лишение прав на чтение файлов](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_22-01-14.png){#fig:019 width=70%}

Лишила себя права на выполнение каталога ~/play, посмотрела как это работает и вернула права обратно.

![Лишение прав на выполнение каталога](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_22-02-13.png){#fig:020 width=70%}

4. Затем я прочитала man по командам mount, fsck, mkfs, kill.

![Просмотр mount](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_22-02-57.png){#fig:021 width=70%}

![Просмотр fsck](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_22-03-50.png){#fig:022 width=70%}

![Просмотр mkfs](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_22-04-39.png){#fig:023 width=70%}

![Просмотр kill](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab07/report/image/2025-03-25_22-05-13.png){#fig:024 width=70%}

# Выводы

Я ознакомилась с файловой системой Linux, её структурой, именами и содержанием каталогов приобрела практические навыки по применению команд для работы с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы. 



