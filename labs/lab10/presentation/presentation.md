---
title: Лабораторная работа №10
subtitle: Текстовой редактор vi
author:
  - Прозорова Е. Е.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 15 апреля 2025 

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Прозорова Елизавета Евгеньевна
  * студент факультета ФМиЕН
  * группа НММбд-03-24
  * Российский университет дружбы народов
  * [1132246767@pfur.ru](mailto:1132246767@pfur.ru)

:::
::: {.column width="30%"}

:::
::::::::::::::

# Вводная часть

## Цели и задачи

- Познакомиться с операционной системой Linux. 
- Получить практические навыки работы с редактором vi, установленным по умолчанию практически во всех дистрибутивах.

# Выполнение лабораторной работы

## Я ознакомилась с редактором vi.

![man vi](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_18-43-57.png){#fig:001 width=70%}

# Задание 1. 

## Создала каталог, перешла в этот каталог

![Каталог](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_18-55-17.png){#fig:002 width=70%}

## Я открыла редактор vi и создала файл hello.sh:

![файл hello.sh](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_18-56-07.png){#fig:003 width=70%}

## Я ввела hello текст.

![Hello текст](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_18-57-04.png){#fig:004 width=70%}

## Ввела wq, сохранив изменения и закрыв редактор.

![Ввод wq](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_19-01-01.png){#fig:005 width=70%}

## Сделала файл исполняемым.

![файл исполняем](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_19-01-46.png){#fig:006 width=70%}

# Задание 2. 

## Открыла файл на редактирование

![Рекактор vi](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab09/report/image/2025-04-08_21-49-48.png){#fig:007 width=70%}

## Я исправила HELL на HELLO

![Изменения текста](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_19-09-23.png){#fig:008 width=70%}

## Перешла на последнюю строку, ниже ввела echo $HELLO

![Изменения текста](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_19-13-22.png){#fig:009 width=70%}

## Удалила последнюю строку, с помощью команды dd

![Изменения текста](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_19-36-08.png){#fig:010 width=70%}

## Затем я отмените удаление с помощью u. на этом я всё сохранила и закрыла редактор

![Итоговый измененный текст](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab10/report/image/2025-04-15_19-36-56.png)){#fig:011 width=70%}

# Выводы

В ходе работы освоены основы использования редактора vi в Linux: создание, редактирование и сохранение файлов. Получены базовые навыки работы в терминальной среде.

:::

