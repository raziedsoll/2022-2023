---
# Front matter
lang: ru-Ru
title: "Лабораторная работа №1"
subtitle: "Установка дистрибутива Rocky"
author: "Аль-Дорихим Рамзи"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: xelatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Приобретение практических навыков установки операционной системы Rocky Linux на виртуальную машину и настройка минимально необходимого окружения для дальнейшей работы.

# Задание

Установить дистрибутив Rocky Linux на виртуальную машину.

# Теоретическое введение

Для выполнения данной лабораторной нет специальной теории. Необходимы общие знания в области компьютерных наук.

# Выполнение лабораторной работы

Создаем виртуальную машину в VirtualBox. 

![Создание виртуальной машины](2022-09/1.JPG){#fig:001}

Указываем объем оперативной памяти, выделенный виртуальной машине.

![Объем оперативной памяти](2022-09/2.JPG){#fig:002}

Создаем новый динамический виртуальный жесткий диск типа VDI и задаем его размер.

![Создание виртуального жесткого диска](2022-09/3.JPG){#fig:003}

![Тип виртуального жесткого диска](2022-09/4.JPG){#fig:004}

![Формат хранения](2022-09/5.JPG){#fig:005}

![Выбор образа операционной системы](2022-09/6.JPG){#fig:006}

В VirtualBox  добавляем новый привод оптических дисков, где выбираем заранее скачанный образ выбранной операционной системы.

![Выбор образа операционной системы](2022-09/8.JPG){#fig:007}

После этого запускаем виртуальную машину и начинаем установку ОС.

![Старт установки ОС](2022-09/9.JPG){#fig:008}

По ходу начальной настройки ОС перед ее установкой нужно выполнить несколько шагов.

​	1. Выбрать язык

![Выбор языка](2022-09/10.png){#fig:009}

2) Настроить часовой пояс.

![Выбор часового пояса](2022-09/14.png){#fig:010}

​	3. Выбрать пакет предустановленных программ.

![Выбор пакета программ](2022-09/19.png){#fig:011}

4. Отключить KDUMP.

![Отключение KDUMP](2022-09/18.png){#fig:011}

5. Включить сетевое соединение.

![Включение сетевого соединения](2022-09/11.png){#fig:012}

6. Установить пароль для root.

![Задание пароля для root](2022-09/13.png){#fig:013}

7. Создать пользователя с правами администратора.

![Создание пользователя](2022-09/17.png){#fig:014}

8. Правильно перезагрузить систему.

![Перезагрузка системы](2022-09/20.png){#fig:015}

После выполнения данных шагов мы попадаем на рабочий стол нашей виртуальной машины. 

![Рабочий стол](2022-09/22.png){#fig:016}

Подключить образ диска дополнительной гостевой ОС.

![Подключение диска дополнительной гостевой ОС](2022-09/24.png){#fig:017}

Процесс подключения.

![Подключение диска дополнительной гостевой ОС](2022-09/23.png){#fig:018}

## Домашнее задание

Информация о системе:

![Информация о системе](2022-09/25.png){#fig:019}

По каким то причинам я не смог получить информацию о текущей тактовой частоте процессора и об доступной памяти.

# Выводы

В ходе выполнения данной лабораторной работы я приобрел  навыки установки операционной системы Rocky Linux на виртуальную машину.


# Список литературы

- <code>[Кулябов Д. С., Королькова А. В., Геворкян М. Н Лабораторная работа №1](https://esystem.rudn.ru/mod/folder/view.php?id=892013)</code>