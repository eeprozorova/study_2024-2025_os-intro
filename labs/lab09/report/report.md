---
## Front matter
title: "Лабораторная работа №9"
subtitle: "Командная оболочка Midnight Commander"
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

Освоение основных возможностей командной оболочки Midnight Commander. Приобретение навыков практической работы по просмотру каталогов и файлов; манипуляций с ними.

# Выполнение лабораторной работы

1. Для начала я изучила информацию о mc, вызвав в командной строке man mc

![man mc](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/2025-04-08_21-41-52.png){#fig:001 width=70%}

2. Запустила из командной строки mc, изучила его структуру и меню

![Команда mc](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/2025-04-08_21-43-06.png){#fig:002 width=70%}

3. Выполнила несколько операций в mc, используя управляющие клавиши 

![Пример: копирование каталога](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/2025-04-08_21-44-13.png){#fig:003 width=70%}

4. Выполните основные команды меню левой (или правой) панели. Оцените степень подробности вывода информации о файлах.

![Левая панель](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/2025-04-08_21-45-46.png){#fig:004 width=70%}

5. Используя возможности подменю Файл , я выполнила следующие задания.

![Ввод имени файла](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/2025-04-08_21-47-14.png){#fig:005 width=70%}

6. С помощью соответствующих средств подменю Команда осуществите следующие задания

![Поиск файлов](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/2025-04-08_21-48-25.png){#fig:006 width=70%}

7. Вызвала подменю Настройки . Освоила операции, определяющие структуру экрана mc

![Настройки mc](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/2025-04-08_21-49-48.png){#fig:007 width=70%}

8. Я создала текстовой файл text.txt.

![Файл text.txt.](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/2025-04-08_21-51-00.png){#fig:008 width=70%}

9. Открыла этот файл с помощью встроенного в mc редактора

![Файл в редакторе](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/2025-04-08_21-54-41.png){#fig:009 width=70%}

10. Я вставила в открытый файл небольшой фрагмент текста

![Текст](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/2025-04-08_21-54-41.png){#fig:010 width=70%}

11. Я проделала с текстом некоторые манипуляции, используя горячие клавиши. Затем я сохранила файл.

![Измененный текст](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/2025-04-08_21-56-16.png)){#fig:011 width=70%}

12. Я открыла файл с исходным текстом на языке программирования C

![Файл на языке C](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/2025-04-08_22-14-26.png){#fig:012 width=70%}

13. Используя меню редактора, включила подсветку синтаксиса,

![Подсветка синтенса](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/2025-04-08_22-25-13.png){#fig:013 width=70%}

# Выводы

Я освоила основные возможности командной оболочки Midnight Commander. Приобрела навыки практической работы по просмотру каталогов и файлов; манипуляций с ними.

:::
