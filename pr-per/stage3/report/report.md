---
## Front matter
title: "Индивидуальный проект"
subtitle: "Третий этап"
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

- Добавить к сайту достижения. Список достижений.
    Добавить информацию о навыках (Skills).
    Добавить информацию об опыте (Experience).
    Добавить информацию о достижениях (Accomplishments).
- Добавить пост на тему "Язык разметки Markdown"

# Выполнение лабораторной работы

1. Сначала я открыла codespace через браузер и стала редактировать подтему Skills, достижения и хобби.

![Skills](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/pr-per/stage3/report/image/2025-04-12_15-12-37.png){#fig:001 width=70%}

Также я добавила информацию о языках.

![Языки](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/pr-per/stage3/report/image/2025-04-12_15-13-37.png){#fig:002 width=70%}

2. Теперь я займусь написание поста по теме. Для начала выберу тему.

![Тема поста](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/pr-per/stage3/report/image/2025-04-12_15-14-51.png){#fig:003 width=70%}

Я написала полный текст о Markdown.

![Итоговый текст](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/pr-per/stage3/presentation/image/2025-04-12_15-17-38.png){#fig:004 width=70%}

# Выводы

Итак, я добавила информацию о достижениях и прочем и написала новый пост.

![Мой сайт](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/pr-per/stage3/report/image/2025-03-16_18-55-17.png){#fig:005 width=70%}

:::
