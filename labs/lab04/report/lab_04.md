---
## Front matter
title: "Отчет по лабораторной работе №4"

subtitle: "дисциплина: Архитектура клмпьютера"

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

Освоение процедуры оформления отчетов с помощью легковесного языка разметки Markdown.

# Задание

Изучить легковестный язык разметки Markdown.

# Теоретическое введение

Чтобы создать заголовок, используйте знак #, например: #This is heading 1

Чтобы задать для текста полужирное начертание, заключите его в двойные

звездочки: This text is **bold**

Чтобы задать для текста курсивное начертание, заключите его в одинарные

звездочки:

This text is *italic*.

Чтобы задать для текста полужирное и курсивное начертание, заключите его

в тройные звездочки:

# Выполнение лабораторной работы

1. Я открыла терминал

2. Перешла в каталог курса сформированный при выполнении лабораторной работы No3 и обновила локальный репозиторий: (рис. [-@fig:001])

![Обновила локальный репозиторий: git pull](image/41.png){ #fig:001 width=70% }

3. Перешла в каталог с шаблоном отчета по лабораторной работе No 4 (рис. [-@fig:002])

![Шаблон](image/46.png){ #fig:002 width=70% }

4. Провела компиляцию шаблона с использованием Makefile. (рис. [-@fig:003], рис. [-@fig:004])

![Ввела команду make](image/42.png){ #fig:003 width=70%,}

Сгенерировались файлы report.pdf и report.docx.

![файлы report.pdf и report.docx. ](image/43.png){ #fig:004 width=70% }

5. Удалила полученный файлы с использованием Makefile. (рис. [-@fig:005])

![Ввела команду make clean](image/44.png){ #fig:005 width=70% }

6. Открыла файл report.md c помощью текстового редактора gedit (рис. [-@fig:006], рис. [-@fig:007])

![Открыла редактор](image/45.png){ #fig:006 width=70% }

![Открыла редактор](image/46.png){ #fig:007 width=70% }

7. Заполнила отчет и скомпилировала отчет с использованием Makefile. (рис. [-@fig:008], рис. [-@fig:009],)

![Заполнила отчет](image/90.png){ #fig:008 width=70% }

![Команда make](image/91.png){ #fig:009 width=70% }


8. Загрузила файлы на Github.(рис. [-@fig:010],)

![github загрузка](image/gith.png){ #fig:010 width=70% }


# Самостоятельная работа

1. Сделала отчёт по лабораторной работе No 3 в формате Markdown.

Заполнила отчет и скомпилировала отчет с использованием Makefile. (рис. [-@fig:011], рис. [-@fig:012], рис. [-@fig:013]

![Заполнила отчет](image/47.png){ #fig:011 width=70% }

![Команда make](image/ytn.png){ #fig:012 width=70% }

![Проверила корректность полученных файлов](image/48.png){ #fig:013 width=70% }

2. Загрузила файлы на github. (рис. [-@fig:014], рис. [-@fig:015], рис. [-@fig:016]

![Загрузка на github](image/49.png){ #fig:014 width=70% }

![Загрузка на github](image/50.png){ #fig:015 width=70% }

![Загрузка на github](image/51.png){ #fig:016 width=70% }


# Выводы

Я освоила процедуры оформления отчетов с помощью легковесного языка разметки Markdown.

# Список литературы{.unnumbered}

::: {#refs}
:::
