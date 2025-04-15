---
## Front matter
title: "Лабораторная работа №9"
subtitle: "Текстовой редактор vi"
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

- Познакомиться с операционной системой Linux. 
- Получить практические навыки работы с редактором vi, установленным по умолчанию практически во всех дистрибутивах.

# Выполнение лабораторной работы

Я ознакомилась с редактором vi.

![man vi](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_18-43-57.png){#fig:001 width=70%}

## Задание 1. 

1. Создала каталог, перешла в этот каталог

![Каталог](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_18-55-17.png){#fig:002 width=70%}

2. Я открыла редактор vi и создала файл hello.sh:

![файл hello.sh](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_18-56-07.png){#fig:003 width=70%}

3.  Я ввела hello текст.

![Hello текст](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_18-57-04.png){#fig:004 width=70%}

4. Ввела wq, сохранив изменения и закрыв редактор.

![Ввод wq](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_19-01-01.png){#fig:005 width=70%}

5. Сделала файл исполняемым.

![файл исполняем](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_19-01-46.png){#fig:006 width=70%}

## Задание 2. 

1. Открыла файл на редактирование

![Рекактор vi](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/2025-04-08_21-49-48.png){#fig:007 width=70%}

2. Я исправила HELL на HELLO

![Изменения текста](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_19-09-23.png){#fig:008 width=70%}

3. Перешла на последнюю строку, ниже ввела echo $HELLO

![Изменения текста](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_19-13-22.png){#fig:009 width=70%}

4. Удалила последнюю строку, с помощью команды dd

![Изменения текста](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_19-36-08.png){#fig:010 width=70%}

5. Затем я отмените удаление с помощью u. на этом я всё сохранила и закрыла редактор

![Итоговый измененный текст](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_19-36-56.png)){#fig:011 width=70%}

# Выводы

В ходе работы освоены основы использования редактора vi в Linux: создание, редактирование и сохранение файлов. Получены базовые навыки работы в терминальной среде.

:::
