---
## Front matter
title: "Индивидуальный проект"
subtitle: "Второй этап"
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

Добавить к сайту данные о себе.    
   Список добавляемых данных.
        -   Разместить фотографию владельца сайта.
        -   Разместить краткое описание владельца сайта (Biography).
        -   Добавить информацию об интересах (Interests).
        -   Добавить информацию от образовании (Education).
    Сделать пост по прошедшей неделе.
    Добавить пост на тему по выбору:
        -   Управление версиями. Git.

# Выполнение лабораторной работы

1.  Сначала я открыла codespace через браузер и открыла папку content/authors/admin/_index.md

![_index.md](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/pr-per/stage2/report/image/2025-03-16_18-48-23.png){#fig:001 width=70%}

Я заменила title, bio и данные автора/админа на свои.

![Моё имя](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/pr-per/stage2/report/image/2025-03-16_18-49-26.png){#fig:002 width=70%}

Я добавила информацию об интересах (Interests)

![Мои интересы](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/pr-per/stage2/report/image/2025-03-16_18-50-51.png){#fig:003 width=70%}

Я добавила информацию от образовании (Education)

![Данные о моем образовании](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/pr-per/stage2/report/image/2025-03-16_18-51-41.png){#fig:004 width=70%}

Я заменила фото из шаблона на своё фото, переименовала файл с моим фото в avatar.

![Моё фото](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/pr-per/stage2/report/image/2025-03-16_18-53-17.png){#fig:005 width=70%}

Я сделала пост по теме "Управление версиями. Git."

![Мой пост](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/pr-per/stage2/report/image/2025-03-16_18-54-41.png){#fig:006 width=70%}

# Выводы

Вот так выглядит мой сайт на втором этапе проекта.

![Мой сайт](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/pr-per/stage2/report/image/2025-03-16_18-55-17.png){#fig:007 width=70%}

