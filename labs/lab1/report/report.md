---
# Front matter
lang: ru-RU
title: "Лабораторная работа №1"
subtitle: "Работа с git"
author: "Логинов Егор Игоревич"

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
pdf-engine: lualatex
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

Вспомнить основные навыки работы с git через терминал и веб-сервер, настроить рабочее пространство, в котором в последствии будем выполнять лабораторные работы. Ознакомиться с языком разметки markdown.

# Задание

1. Настройку рабочего пространства на Github.
2. Выполнить задания, которые указаны в файле git.pdf
3. Cоставить отчёт по проделанной работе в форматах pdf, d согласно рекомендациям из файла markdown

# Теоретическое введение

Git — система управления версиями с распределенной архитектурой. В отличие от некогда популярных систем вроде CVS и Subversion (SVN), где полная история версий проекта доступна лишь в одном месте, в Git каждая рабочая копия кода сама по себе является репозиторием. Это позволяет всем разработчикам хранить историю изменений в полном объеме.

Разработка в Git ориентирована на обеспечение высокой производительности, безопасности и гибкости распределенной системы.

# Выполнение лабораторной работы

1. Создали репозиторий на Github, чтобы сохранять там наши изменения. Далее клонируем его и создадим все файлы для нашего курса.

![Github репозиторий](image/fig001.png){ #fig:001 } 

2. Создали рабочее пространство для лабораторных работ, групповых проектов и т.д.

![Схема рабочего пространства](image/fig002.png){ #fig:002 width=70%}

3. Запустим скрипт автоматического развертывания рабочего пространства, создания папок, лабораторных работ и отчетов. Отправим все эти изменения на Github.

![Просмотр появившихся изменений](image/fig003.png){ #fig:003 width=70%}

4. На удаленном репозитории можно увидеть отправленные изменения.

![Удаленный репозиторий](image/fig004.png){ #fig:004 width=70%}

5. Установил имя, электронную почту github, параметры установки окончаний строк и отображение unicode

![Установка имени и почты](image/fig005.png){ #fig:005 width=70%}

![Установка параметров](image/fig006.png){ #fig:006 width=70%}

6. Создал директорию hello, в которой создал файл hello.html. В этом файле написал "Hello, World!"

![Создание файла hello.html](image/fig007.png){ #fig:007 width=70%}

7. Добавил файл в репозиторий.

![Добавление файла в репозиторий](image/fig008.png){ #fig:008 width=70%}

8. Изменил файл hello.html, добавив HTML теги. Проиндексировал изменения и сделал коммит изменений.

![Добавление HTML тегов](image/fig009.png){ #fig:009 width=70%}

![Коммит изменений](image/fig010.png){ #fig:010 width=70%}

9. Изменил hello.html, добавив теги html и body. Проиндексировал изменения и сделал коммит изменений.

![Добавление тегов](image/fig011.png){ #fig:011 width=70%}

![Индексация изменений](image/fig012.png){ #fig:012 width=70%}

10. Получил список произведенных изменений.

![Список изменений](image/fig013.png){ #fig:013 width=70%}

11. Получил старую версию проекта с помощью хэша предыдущей версии.

![Получение старой версии](image/fig014.png){ #fig:014 width=70%}

12. Вернулся к последней версии в ветке master, проверил файл hello.html. Создал тег v1 для этой версии.

![Получение последней версии](image/fig015.png){ #fig:015 width=70%}

![Список изменений](image/fig016.png){ #fig:016 width=70%}

13. Переключился между тегами веток.

![Переключение между тегами](image/fig017.png){ #fig:017 width=70%}

14. Переключился на ветку master, изменил файл hello.html. После этого отменил локальные изменения.

![Отмена локальных изменений](image/fig018.png){ #fig:018 width=70%}

15. Отменил изменения в рабочем каталоге.

![Отмена изменений в рабочем каталоге](image/fig019.png){ #fig:019 width=70%}

16. Изменил файл hello.html и сделал коммит. Сделал коммит с новыми изменениями, отменяющими предыдущие. Посмотрел список изменений.

![Удаление нежелательных коммитов](image/fig019.png){ #fig:019 width=70%}

17. Изменил hello.html, а затем сделал коммит.  Изменил предыдущий коммит, добавив email.

![Добавление коммита](image/fig020.png){ #fig:020 width=70%}

![Изменение коммита](image/fig021.png){ #fig:021 width=70%}

18. Переместил файл hello.html в директорию lib. Добавил файл index.html.

![Перемещение файла](image/fig022.png){ #fig:022 width=70%}

![Файл index.html](image/fig023.png){ #fig:023 width=70%}

19. Изучил, как выглядит git внутри.

![Git внутри](image/fig024.png){ #fig:024 width=70%}

![Директории git'a](image/fig025.png){ #fig:025 width=70%}

20. Вывел последний коммит с помощью SHA1 хэша. Вывел каталог lib и файл hello.html.

![Вывод коммита](image/fig026.png){ #fig:026 width=70%}

![Вывод файла hello.html](image/fig027.png){ #fig:027 width=70%}

21. Создал новую ветку style. Добавил новый файл style.css. Посмотрел список изменений.

![Создание новой ветки](image/fig028.png){ #fig:028 width=70%}

![Вывод файла hello.html](image/fig029.png){ #fig:029 width=70%}

22. Переключился на ветку мастер и изменил файл hello.html. Посмотрел graph log. 

![Переключение на ветку master](image/fig030.png){ #fig:030 width=70%}

![Список изменений](image/fig031.png){ #fig:031 width=70%}

23. Сделал слияние веток и посмотрел список изменений.

![Слияние веток](image/fig032.png){ #fig:032 width=70%}

24. Создал конфликт, изменив еще раз файл hello.html. Посмотрел список изменений.

![Список изменений при конфликте](image/fig033.png){ #fig:033 width=70%}

25. Вручную разрешил конфликт в файле hello.html, сделал коммит решения конфликта.

![Решение конфликта](image/fig034.png){ #fig:034 width=70%}

![Список изменений после решения конфликта](image/fig035.png){ #fig:035 width=70%}

26. Сбросил ветку style и посмотрел список изменений.

![Сброс ветки style](image/fig036.png){ #fig:036 width=70%}

27. Аналогично Сбросил ветку master и посмотрел список изменений.

![Сброс ветки master](image/fig037.png){ #fig:037 width=70%}

28. Перебазировал ветку style и посмотел список изменений.

![Список изменений после перебразирования](image/fig038.png){ #fig:038 width=70%}

29. Произвел слияние style в master, посмотрел список изменений

![Список изменений после слияния](image/fig039.png){ #fig:039 width=70%}

30. Клонировал репозиторий mathmod. 

![Клонирование репозитория](image/fig040.png){ #fig:040 width=70%}

31. Посмотрел список удаленных веток. 

![Список удаленных веток](image/fig041.png){ #fig:041 width=70%}

32. Внёс изменения в оригинальный репозиторий, извлёк данные изменения и добавил их в клонированный репозиторий.

![Извлечение изменений](image/fig042.png){ #fig:042 width=70%}

# Выводы

Я получил основные навыки работы с git через терминал и веб-сервер, настроил рабочее пространство, в котором в последствии буду выполнять лабораторные работы. Ознакомился с языком разметки markdown.

# Список литературы

Использовал приложенные к работе файлы: git.pdf, markdown.pdf
