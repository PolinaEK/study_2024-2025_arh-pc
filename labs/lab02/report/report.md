---
## Front matter
title: "Отчет по лабораторной работе №2"
subtitle: "дисциплина: Архитектура компьютеров"
author: "Кичигина Полина Евгеньевна"

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

Целью работы является изучение идеологии и применение средств контроля версий.
Приобретение практических навыков с системой git.


# Выполнение лабораторной работы
Задание №1 Базовая настройка git

1. Сначала сделаем предварительную конфигурацию git(рис. [-@fig:001])

![Задаём имя и email репозитория.](image/1.png){#fig:001 width=70%}

2. Настроим utf-8 в выводе сообщений git(рис. [-@fig:002])

![Настраиваем utf-8.](image/2.png){#fig:002 width=70%}

3. Зададим имя начальной ветки (будем называть её master)(рис. [-@fig:003])

![Зададим имя начальной ветки (master)](image/3.png){#fig:003 width=70%}

4. Параметр autocrlf(рис. [-@fig:004])

![Устанавливаем параметр autocrlf.](image/4.png){#fig:004 width=70%}

5. Параметр safecrlf(рис. [-@fig:005])

![Устанавливаем настройку safecrlf.](image/5.png){#fig:005 width=70%}


Задание №2. Создание SSH ключа.

Для последующей идентификации пользователя на сервере репозиториев

необходимо сгенерировать пару ключей (приватный и открытый)(рис. [-@fig:006])

![Генерируем пару ключей.](image/6.png){#fig:006 width=70%}

Далее необходимо загрузить сгенерённый ключ(рис. [-@fig:007])

![Копируем ключ из локальной сети в буфер обмена.](image/7.png){#fig:007 width=70%}

Заходим в свой аккаунт на сайте github и переходим в настройки(рис. [-@fig:008])

![Добавляем скопированный ключ и указываем имя ключа (Title).](image/8.png){#fig:008 width=70%}


Задание №3. Создание рабочего пространства и репозитория курса на основе
шаблона.

Открываем терминал для создания рабочего пространства(рис. [-@fig:009])

![Создаём каталог для предмета «Архитектура компьютера».](image/9.png){#fig:009 width=70%}


Задание №4. Создание репозитория курса.

Переходим на страницу репозитория с шаблоном(рис. [-@fig:010])

![Создаём репозиторий по шаблону и называем его «study_2024–2025_arh-pc».](image/10.png){#fig:010 width=70%}

Открываем терминал(рис. [-@fig:011])

![Переходим в каталог курса и клонируем созданный репозиторий.](image/11.png){#fig:011 width=70%}


Задание №5. Настройка каталога курса.

Переходим в каталог курса(рис. [-@fig:012])

![Перешли в каталог курса.](image/12.png){#fig:012 width=70%}

Отправьте файлы на сервер(рис. [-@fig:013])

![Отправка файлов на сервер.](image/13.png){#fig:013 width=70%}

# Задания для самостоятельной работы

1.Создайте отчет по выполнению лабораторной работы в соответствующем каталоге
рабочего пространства (labs>lab02>report)(рис. [-@fig:014])

![создаем файл для отчета.](image/14.png){#fig:014 width=70%}

2. Скопируйте отчеты по выполнению предыдущих лабораторных работ в соответствующие каталоги созданного рабочего пространства. (рис. [-@fig:015])

![Копирование отчета по лабораторной работе в нужный каталог.](image/15.png){#fig:015 width=70%}

3. Загрузите файлы на github (рис. [-@fig:016]) 

![Добавление файлов с помощью команды git add и touch.](image/16.png){#fig:016 width=70%}

(рис. [-@fig:017])

![Команда git push для завершения копирования.](image/17.png){#fig:017 width=70%}

# Выводы

В ходе выполнения лабораторной работы мы познакомились с системой контроля git, выучили команды для работы с ним, создали свой репозиторий на платформе github, где в последствии будут храниться все будущие отчёты по лабораторным работам.


