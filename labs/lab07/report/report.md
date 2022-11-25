---
## Front matter
title: "Лабораторная работа №7"
subtitle: "Архитектура компьютера"
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

Освоение арифметических инструкций языка ассемблера NASM

# Задание

Освоиьть арифметические инструкции языка ассемблера NASM

# Теоретическое введение

Регистровая адресация – операнды хранятся в регистрах и в команде используются имена этих регистров, например: mov ax,bx.

Непосредственная адресация – значение операнда задается непосредственно в команде, Например: mov ax,2

# Выполнение лабораторной работы

1. Создала каталог для программам лабораторной работы No 7, перешла в него и создала файл lab7-1.asm:(рис. [-@fig:001])

![создала файл lab7-1.asm](image/Снимок экрана от 2022-11-24 10-53-37.png){ #fig:001 width=70% }

2. Ввела в файл lab7-1.asm текст программы из листинга 7.1

Создала исполняемый файл и запустила его.(рис. [-@fig:002])

![результат символ j.](image/Снимок экрана от 2022-11-24 11-14-05.png){ #fig:002 width=70% } 

3. Далее изменила текст программы и вместо символов, записала в регистры числа. (рис. [-@fig:003])

![Исправила текст программы следующим образом:](image/Снимок экрана от 2022-11-24 11-15-40.png){ #fig:003 width=70% }

Создала исполняемый файл и запустила его.(рис. [-@fig:004])

![Вывелся символ с кодом 10](image/Снимок экрана от 2022-11-24 11-21-05.png){ #fig:004 width=70% }

Символ при выводе на экран не отображается

4. Создала файл lab7-2.asm и ввела в него текст программы из листинга 7.2.(рис. [-@fig:005; -@fig:006])

![Файл lab7-2.asm](image/Снимок экрана от 2022-11-24 11-22-08.png){ #fig:005 width=70% }

Создала исполняемый файл и запустила его

![Получила число 106.](image/Снимок экрана от 2022-11-24 11-25-36.png ){ #fig:006 width=70% }

5. Изменила символы на числа. (рис. [-@fig:007; -@fig:008; -@fig:009; -@fig:010])

![Изменение](image/Снимок экрана от 2022-11-24 11-26-32.png){ #fig:007 width=70% }

Создала исполняемый файл и запустила его. 

![Результат 10](image/Снимок экрана от 2022-11-24 11-27-57.png){ #fig:008 width=70% }

Заменила функцию iprintLF на iprint.

![iprintLF на iprint](image/Снимок экрана от 2022-11-24 11-28-46.png){ #fig:009 width=70% }


![Результат](image/Снимок экрана от 2022-11-24 11-30-04.png){ #fig:010 width=70% }

7.3.2. Выполнение арифметических операций в NASM

6. Создала файл lab7-3.asm. Ввела текст программы из листинга 7.3  в lab7-3.asm.(рис. [-@fig:011])

![Создала исполняемый файл и запустила его. ](image/Снимок экрана от 2022-11-24 11-37-03.png){ #fig:011 width=70% }

Изменила текст программы для вычисления выражения y=(4*6+2)/5 (рис. [-@fig:012; -@fig:013])

![Текст](image/Снимок экрана от 2022-11-24 11-39-52.png){ #fig:012 width=70% }

![Создала исполняемый файл и запустила его](image/Снимок экрана от 2022-11-24 11-41-28.png){ #fig:013 width=70% }

7. Создала файл variant.asm. Ввела текст программы из листинга 7.4 в файл variant.asm.(рис. [-@fig:014])

![Создала исполняемый файл и запустила его. ](image/Снимок экрана от 2022-11-25 13-39-59.png){ #fig:014 width=70% }

1. Какие строки листинга 7.4 отвечают за вывод на экран сообщения ‘Ваш вариант:’? 

mov eax, msg call sprintLF

2. Для чего используется следующие инструкции? nasm mov ecx, xmov edx, 80 call sread

Для ввода переменной X с клавиатуры и сохранения введенных данных

3. Для чего используется инструкция “call atoi”?

Для преобраззования кода переменной ASCII в число

4. Какие строки листинга 7.4 отвечают за вычисления варианта?

mov ebx, 20 div ebx, inc edx

5. В какой регистр записывается остаток от деления при выполнении инструкции “div ebx”?

ebx

6. Для чего используется инструкция “inc edx”?

 Для увеличения значения edx на 1
 
7. Какие строки листинга 7.4 отвечают за вывод на экран результата вычислений?

mov eax, edx call iprint LF

7.4. Задание для самостоятельной работы

1. Написала программу вычисления выражения y=(8x+6)10. рис. [-@fig:015; -@fig:016])

![Программа](image/Снимок экрана от 2022-11-25 14-37-57.png){ #fig:015 width=70% }

![Проверила его работу для значений х=1 и х=4](image/Снимок экрана от 2022-11-25 14-33-31.png){ #fig:016 width=70% }

# Выводы

Я освоила арифметические инструкции языка ассемблера NASM

# Список литературы{.unnumbered}

::: {#refs}
:::
