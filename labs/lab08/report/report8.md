---
## Front matter
title: "Лабораторная работа №8"
subtitle: "Поиск файлов. Перенаправление ввода-вывода. Просмотр запущенных процессов"
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

Ознакомление с инструментами поиска файлов и фильтрации текстовых данных.
Приобретение практических навыков: по управлению процессами (и заданиями), по
проверке использования диска и обслуживанию файловых систем.

# Выполнение лабораторной работы

1. Я осуществите вход в систему, используя соответствующее имя пользователя.

2. Я записала в файл file.txt названия файлов, содержащихся в каталоге /etc. Затем я дописала в этот же файл названия файлов, содержащихся в домашнем каталоге.

![Запись  в файл file.txt названия файлов, содержащихся в каталоге /etc и домашнем каталоге](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/2025-04-02_18-56-25.png){#fig:001 width=70%}

3. Я вывела имена всех файлов из file.txt, имеющих расширение .conf, после чего записала их в новый текстовой файл conf.txt 

![Вывод имена всех файлов из file.txt и запись из в файл conf.txt](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/2025-04-02_18-57-55.png){#fig:002 width=70%}

4. Я определила, какие файлы в домашнем каталоге имеют имена, начинавшиеся с символа c двумя способами.

![Первый способ](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/2025-04-02_19-00-37.png){#fig:003 width=70%}

![Второй способ](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/2025-04-02_19-04-29.png){#fig:004 width=70%}

5. Я вывела на экран (по странично) имена файлов из каталога /etc, начинающиеся с символа h.

![Имена файлов начинающиеся с символа](//home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/2025-04-02_19-06-18.png){#fig:005 width=70%}

6. Я запустила в фоновом режиме процесс, который будет записывать в файл ~/logfile файлы, имена которых начинаются с log. Затем удалила файл ~/logfile.

![Фаил ~/logfile](//home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/2025-04-02_19-12-49.png{#fig:006 width=70%}

7. Я запустила из консоли в фоновом режиме редактор gedit.

![gedit в фоновом режиме](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/2025-04-02_19-14-20.png){#fig:007 width=70%}

8. Я определила идентификатор процесса gedit, используя команду ps, конвейер и фильтр grep.

![Фильтр grep](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/2025-04-02_19-14-35.png){#fig:008 width=70%}

Я также попробовала для этого задания команду pgrep

![Команда pgrep](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/2025-04-02_19-15-04.png){#fig:009 width=70%}

9. Я прочла справку (man) команды kill, после чего использовала её для завершения процесса gedit

![Справка kill](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/2025-04-02_19-15-48.png){#fig:010 width=70%}

![Завершения процесса gedit](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/2025-04-02_19-17-04.png)){#fig:011 width=70%}

10. Я выполнила команды df и du, предварительно получив более подробную информацию об этих командах, с помощью команды man.

![Команда df](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/2025-04-02_19-18-23.png){#fig:012 width=70%}

![Команда du](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/2025-04-02_19-19-03.png){#fig:013 width=70%}

11. Воспользовавшись справкой команды find, вывела имена всех директорий, имеющихся в домашнем каталоге.

![Все директории](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab08/report/image/2025-04-02_19-21-00.png){#fig:014 width=70%}

# Выводы

Я ознакомилась инструментами поиска файлов и фильтрации текстовых данных. Я приобрела практические навыки по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.

