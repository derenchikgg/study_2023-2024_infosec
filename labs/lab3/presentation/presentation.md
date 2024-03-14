---
## Front matter
lang: ru-RU
title: Лабораторная работа 
subtitle: Дискреционное разграничение прав в Linux. Два пользователя
author:
  - Панченко Д. Д.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 14 марта 2024

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
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

# Информация

## Докладчик

  * Панченко Денис Дмитриевич
  * Студент 2 курса факультета физико-математических наук.
  * Российский университет дружбы народов
  * [derenchikde@gmail.com](mailto:derenchikde@gmail.com)

## Цели и задачи

Получение практических навыков работы в консоли с атрибутами файлов для групп пользователей.

## Задание

Получить практические навыки работы в консоли с атрибутами файлов для групп пользователей.

# Выполнение лабораторной работы

## Создаем учётную запись пользователя guest.

![Создание](image/1.png)

## Создаем учётную запись пользователя guest2.

![Создание](image/2.png)

## Добавляем пользователя guest2 в группу guest.

![Группа](image/3.png)

## Осуществляем вход в систему от двух пользователей на двух разных консолях.

![guest](image/4.png)

![guest2](image/5.png)

## Командой pwd определяем директорию, в которой мы находимся.

![guest](image/6.png)

![guest2](image/7.png)

## Определяем в какие группы входят пользователи.

![guest](image/8.png)

![guest2](image/9.png)

## Определяем в какие группы входят пользователи с помощью других команды

![guest](image/10.png)

![guest2](image/11.png)

## Просмотрим содержимое файла group.

![group](image/12.png)

## От имени пользователя guest2 выполним регистрацию пользователя guest2 в группе guest.

![Регистрация](image/13.png)

## Разрешим все действия для пользователей группы.

![Разрешение](image/14.png)

## Снимем с директории /home/guest/dir1 все атрибуты.

![Снятие атрибутов](image/15.png)

# Вывод

Я получил практические навыки работы в консоли с атрибутами файлов для групп пользователей.
