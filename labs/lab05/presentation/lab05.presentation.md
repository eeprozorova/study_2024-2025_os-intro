---
## Front matter
lang: ru-RU
title: Лабораторная работа № 5
subtitle: Менеджер паролей pass
author: 
  - Прозорова Е. Е.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 15 марта 2025

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

-   Настройка рабочей среды. 
-   Освоить умения по работе с менеджером паролей pass
-   Изучить идеологию и управление файлами конфигурации.

# Выполнение лабораторной работы

##  Установка pass и gopass.

Сначала я установила менеджер паролей: pass и gopass.

![Установка pass](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-20-53.png)

![Установка gopass](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-23-26.png)

## Инициализация хранилища

 Я вывела список ключей gpg, убедилась что у меня уже есть один. Затем я инициализировала хранилище.

![Инициализация хранилища](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-26-14.png)

Теперь я создала структуру git.

![Синхронизация с git](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-27-34.png)

Также задала адрес репозитория на хостинге (репозиторий создала предварительно)

![адрес репозитория на хостинге](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-30-21.png)

Выполнила команды для синхронизации.

![команда для синхронизации](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-35-11.png)

Я также решила для проверки вручную закоммитить и выложить изменения.

![Прямые изменения](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-36-09.png)

## Native messaging

Я скачала интерфейс для взаимодействия с браузером (native messaging)

![browserpass](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-41-26.png)

## Дополнительное программное обеспечение

 Установила дополнительное программное обеспечение.

![Дополнительное программное обеспечение](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-43-07.png)

Затем я установила шрифты.

![Установка шрифтов](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-44-35.png)

## Установка бинарного файла

Я установила бинарный файл с помощью `wget`

![Установка бинарного файла](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-48-54.png)

## Инициализация chezmoi

Инициализировала `chezmoi` со своим репозиторием `dotfiles`

![Подключение репозитория к системе](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-51-44.png)

Проверила, какие изменения внёс `chezmoi` в домашний каталог

![Проверка](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-53-51.png)

## Проверка функции автоматического фиксирования.

Включила функцию автоматического фиксирования и отправления изменений в исходный каталог в репозиторий.

![функция автоматического фиксирования](/home/eeprozorova/work/study/2024-2025/Операционные системы/os-intro/labs/lab05/report/image/2025-03-14_18-55-48.png)

# Выводы

Я установила и освоила менеджер паролей, управление файлами конфигурации и установила дополнительное программное обеспечение.
