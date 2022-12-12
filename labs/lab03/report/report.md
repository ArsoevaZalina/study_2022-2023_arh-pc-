---
## Front matter
title: "3. Лабораторная работа No3."
subtitle: " Язык разметки Markdown"
author: "Арсоева Залина НБИбд-01-21"

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

Целью работы является освоение процедуры оформления отчетов с помощью легковесного языка разметки Markdown.

# Задание

1. Откройте терминал

2. Перейдите в каталог курса сформированный при выполнении лабораторной работы No3:

**cd ~/work/study/2022-2023/"Архитектура компьютера"/arch-pc/**

Обновите локальный репозиторий, скачав изменения из удаленного репозитория с помощью команды

**git pull**

3. Перейдите в каталог с шаблоном отчета по лабораторной работе No4

**cd ~/work/study/2022-2023/"Архитектура компьютера"/arch-pc/labs/lab04/report**

4. Проведите компиляцию шаблона с использованием Makefile. Для этого введите команду

**make**

При успешной компиляции должны сгенерироваться файлы report.pdf и report.docx. Откройте и проверьте корректность полученных файлов.

5. Удалите полученный файлы с использованием Makefile. Для этого введите команду

**make clean**

Проверьте, что после этой команды файлы report.pdf и report.docx были удалены.

6. Откройте файл report.md c помощью любого текстового редактора, например gedit

**gedit report.md**

Внимательно изучите структуру этого файла.

7. Заполните отчет и скомпилируйте отчет с использованием Makefile. Проверьте корректность полученных файлов. (Обратите внимание, для корректного отображения скриншотов они должны быть размещены в каталоге image)

8. Загрузите файлы на Github.

**cd ~/work/study/2022-2023/"Архитектура компьютера"/arch-pc**
**git add .**
**git commit -am 'feat(main): add files lab-4'**
**git push**

# Задание для самостоятельной работы

1. В соответствующем каталоге сделайте отчёт по лабораторной работе No3 в формате Markdown. В качестве отчёта необходимо предоставить отчёты в 3 форматах: pdf, docx и md.

2. Загрузите файлы на github

# Выполнение лабораторной работы

Описываются проведённые действия, в качестве иллюстрации даётся ссылка на иллюстрацию (рис. [-@fig:001])

![Название рисунка](image/placeimg_800_600_tech.jpg){ #fig:001 width=70% }

1. Открываю терминал. (рис. [-@fig:001])

![Терминал](image/1.jpg){ #fig:001 width=70% }

2. Перехожу в каталог курса сформированный при выполнении лабораторной работы No2:(рис. [-@fig:002])

![Переход в каталог курса ](image/2.jpg){ #fig:002 width=70% }

Обновляю локальный репозиторий, скачав изменения из удаленного репозитория с помощью команды **git pull** (рис. [-@fig:003])

![git pull](image/3.jpg){ #fig:003 width=70% } 

3. Перехожу в каталог с шаблоном отчета по лабораторной работе No4. (рис. [-@fig:004])

![Перехожу в каталог с шаблоном отчета](image/4.jpg){ #fig:004 width=70% } 

4. Проведите компиляцию шаблона с использованием Makefile. Для этого введите команду **make**. При успешной компиляции должны сгенерироваться файлы report.pdf и report.docx. Откройте и проверьте корректность полученных файлов.(рис. [-@fig:005])

![make](image/5.jpg){ #fig:005 width=70% } 

5. Удалите полученный файлы с использованием Makefile. Для этого введите команду **make clean** (рис. [-@fig:006])

![make clean](image/6.jpg){ #fig:006 width=70% } 

Проверьте, что после этой команды файлы report.pdf и report.docx были удалены.(рис. [-@fig:007])

![report.pdf и report.docx удалены](image/7.jpg){ #fig:007 width=70% } 

6. Откройте файл report.md c помощью любого текстового редактора, например gedit **gedit report.md**

(рис. [-@fig:008])

![gedit report.md](image/8.jpg){ #fig:008 width=70% } 

7. Заполните отчет и скомпилируйте отчет с использованием Makefile. Проверьте корректность полученных файлов. (Обратите внимание, для корректного отображения скриншотов они должны быть размещены в каталоге image) (рис. [-@fig:009])

![Заполнение отчета](image/9.jpg){ #fig:009 width=70% } 

8. Загрузите файлы на Github.

**cd ~/work/study/2022-2023/"Архитектура компьютера"/arch-pc**
**git add .**
**git commit -am 'feat(main): add files lab-4'**
**git push**

(рис. [-@fig:0010])

![Загрузка файлов на Github](image/10.jpg){ #fig:010 width=70% } 

# Задание для самостоятельной работы

1. В соответствующем каталоге сделайте отчёт по лабораторной работе No2 в формате Markdown. В качестве отчёта необходимо предоставить отчёты в 3 форматах: pdf, docx и md. (рис. [-@fig:003])

![Отчёт ЛБ №2](image/11.jpg){ #fig:011 width=70% } 

2. Загрузите файлы на github (рис. [-@fig:003])

![Загрузка файлов на github](image/12.jpg){ #fig:012 width=70% } 

# Выводы

Я освоила процедуры оформления отчетов с помощью легковесного языка разметки Markdown. Создала необходимые отчеты. 
