---
## Front matter
title: "Лабораторная работа № 5"
subtitle: "Менеджер паролей pass"
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

-   Настройка рабочей среды. 
-   Освоить умения по работе с менеджером паролей pass
-   Изучить идеологию и управление файлами конфигурации.

# Выполнение лабораторной работы

1.  Сначала я установила менеджер паролей: pass и gopass.

![Установка pass](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-20-53.png){#fig:001 width=70%}

![Установка gopass](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-23-26.png){#fig:002 width=70%}

2. Я вывела список ключей gpg, убедилась что у меня уже есть один. Затем я инициализировала хранилище.

![Инициализация хранилища](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-26-14.png){#fig:003 width=70%}

Теперь я создала структуру git.

![Синхронизация с git](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-27-34.png){#fig:004 width=70%}

Также задала адрес репозитория на хостинге (репозиторий создала предварительно)

![адрес репозитория на хостинге](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-30-21.png){#fig:005 width=70%}

Выполнила команды для синхронизации.

![команда для синхронизации](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-35-11.png){#fig:006 width=70%}

Я также решила для проверки вручную закоммитить и выложить изменения.

![Прямые изменения](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-36-09.png){#fig:007 width=70%}

3. Я скачала интерфейс для взаимодействия с браузером (native messaging)

![browserpass](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-41-26.png){#fig:008 width=70%}

4. Установила дополнительное программное обеспечение.

![Дополнительное программное обеспечение](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-43-07.png){#fig:009 width=70%}

Затем я установила шрифты.

![Установка шрифтов](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-44-35.png){#fig:010 width=70%}

5. Я установила бинарный файл с помощью `wget`

![Установка бинарного файла](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-48-54.png)){#fig:011 width=70%}

6. Инициализировала `chezmoi` со своим репозиторием `dotfiles`

![Подключение репозитория к системе](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-51-44.png){#fig:012 width=70%}

Проверила, какие изменения внёс `chezmoi` в домашний каталог

![Проверка](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-53-51.png){#fig:013 width=70%}

7. Включила функцию автоматического фиксирования и отправления изменений в исходный каталог в репозиторий.

![функция автоматического фиксирования](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-55-48.png){#fig:014 width=70%}

# Выводы

Я установила и освоила менеджер паролей, управление файлами конфигурации и установила дополнительное программное обеспечение.
