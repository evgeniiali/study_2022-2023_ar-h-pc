---
## Front matter

title: "ОТЧЕТ ПО ЛАБОРАТОРНОЙ РАБОТЕ №3"

subtitle: "дисциплина: Архитектура компьютеров"

author: "Ли Евгения Олеговна"

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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
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

Изучить идеологию и применение средств контроля версий. Приобрести практические навыки по работе с системой git.

# Задание

Применить средства контроля версий в работе с системой git. Изучить идеологию системы git.

# Теоретическое введение

Репрозиторий - место, где хранятся данные.

Система контроля версий Git - набор программ из командной строки, доступ к которым получается из терминала с помощью команды git.

# Выполнение лабораторной работы

1. Настройка github

Я создала учетную запись на сайте github.com и заполнила основные данные (рис.[-@fig:001])

![Создание учетной записи](image/1.jpg){ #fig:001 width=70% } 

2. Базовая настройка git 

Ввела в терминал необходимые команды, указав имя и email (рис.[-@fig:002])

![Команды](image/2.jpg){ #fig:002 width=70% }

Настроила utf-8 в выводе сообщений git и Задала имя начальной ветки, Параметр autocrlf:, Параметр safecrlf: (рис.[-@fig:003])

![Параметр safecrlf:](image/3.jpg){ #fig:003 width=70% }

3. Создание SSH ключа

На сервере репозиториев сгенерировала пару ключей (приватный и открытый) (рис.[-@fig:004])

![Сгенерировала пару ключей](image/4.jpg){ #fig:004 width=70% }

Загрузила сгенерённый открытый ключ. (рис.[-@fig:005])

![Загрузила сгенерённый открытый ключ](image/5.jpg){ #fig:005 width=70% }

4. Создание рабочего пространства и репозитория курса на основе шаблона

Создала каталог для предмета «Архитектура компьютера»: (рис.[-@fig:006])

![каталог для предмета «Архитектура компьютера»](image/6.jpg){ #fig:006 width=70% }

5. Создание репозитория курса на основе шаблона

создала через web-интерфейс github.репозиторий курса на основе шаблона и клонировала созданный репозиторий: (рис.[-@fig:007])

![репозиторий курса на основе шаблона, клон](image/7.jpg){ #fig:007 width=70% }

6. Настройка каталога курса

Я перешла в каталог курса, удалила лишние файлы, создала необходимые каталоги: (рис.[-@fig:008], рис.[-@fig:009], рис.[-@fig:010])

![удалила лишние файлы](image/8.jpg){ #fig:008 width=70% }

![создала необходимые каталоги](image/9.jpg){ #fig:009 width=70% }

![make](image/10.jpg){ #fig:010 width=70% }

Отправила файлы на сервер (рис.[-@fig:011]) (рис.[-@fig:012]) (рис.[-@fig:013])

![Отправила файлы на сервер](image/11.jpg){ #fig:011 width=70% }

![Отправила файлы на сервер](image/12.jpg){ #fig:012 width=70% }

![Отправила файлы на сервер](image/13.jpg){ #fig:013 width=70% }

# Задание для Самостоятельной работы

1. Создала отчет по выполнению лабораторной работы в соответствующем каталоге рабочего пространства (labs>lab03>report).

![каталоге рабочего пространства (labs>lab03>report)](image/c1.jpg){ #fig:014 width=70% }

2. Скопировала отчеты по выполнению предыдущих лабораторных работ в соответствующие каталоги созданного рабочего пространства.

![Скопировала отчеты по выполнению предыдущих лабораторных](image/c2.jpg){ #fig:015 width=70% }

3. Загрузила файлы на github.

![Загрузила файлы на github.](image/c3.jpg){ #fig:016 width=70% }


# Выводы

Я изучила идеологию и применение средств контроля версий. Приобрела практические навыки по работе с системой git.

# Список литературы{.unnumbered}

::: {#refs}
:::
