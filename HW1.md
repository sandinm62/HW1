# **Инструкция по работе Git"**

![Git](img/git.png)


## Первоначальная настройки Git

    git config –global user.name “ваше имя для git”
    git config –global user.email “ваш email для git” 

## Создание нового локального репозитория

Для создания нового репозитория (инициализации) нужно ввести команду:
    
    git init

## Chek status repository 

To chek status of a repository, use the command:

    git status

## Добавление файла к отслеживанию

Для добавления файла к отслеживанию нужно ввести команду:

    git add <filename>

## Добавление изменений к отслеживанию

Для добавления изменений к отслеживанию нужно ввести команду:

    git commit

## Добавление изменений с комментарием

Для добавления изменений к отслеживанию с комментарием введите команду с доплнительным индексом _-m_ и в кавычках укажите информацию об изменениях:

    git commit -m "message"

## Добавление файла к отслеживанию после внесения изменений через команду git commit

Для добавления файла к отслеживанию после внесения изменений через команду git commit добавть к данной команде индекс __-a__:

    git commit -a

## Добавление файла к отслеживанию и внесение комментария одной командой

Для добавления файла к отслежеванию после изменений и добавления комментария можно использовать следующую команду:

    git commit -am "message"

## Вывод списка изменний в файле

Для вывода списка изменний в файле введите следующую команду:

    git log

## Вывод списка измений в файле в компактном виде

Для выода списка в компактном виде введите следующую команду:

    git log --oneline

## Вывод списка полного изменений в файле
 
 Если вы вносили изменния в файле (например вернулись к какой то из предыдущих версий файла) и потом решили вренуться обратно то вам поможет следующая команда которая покажет все состояний файла включая состояния до изменения:

    git log --all

Так же можете воспользоваться компактной версией представления списка:

    git log --all --oneline

## Вывод последних изменений после сохранения файла

Для вывода изменений внесённых в файл после сохранения введи команду:

    git diff

Для проверки того что было внесено в файл в определённом сохранённом комментарии введите команду:

    git diff <hash>

А для сравнения состояний файла между размными версиями его сотояние введите:

    git diff <hash1> <hash2>

## Добавление новой ветки

Для смены ветки введите следющую команду:

    git checkout <branch_name>

где \<branch_name\> имя новой ветки.

Для возвращения на ветку master (main) используйте следующую команду:

    git checkout master

## Ветвления

Ветвления в Git нужны для того чтобы ...

## Просмотр имеющихся веток

Для просмотра всех имеющихся веток нужно ввести команду:

    git branch

## Создание новой ветки

Чтобы создать новую ветку нужно ввести команду:

    git branch <branch name>
где \<branh name\> это имя новой ветки
 
## Объединение веток
  
Для того чтобы влить изменения из одной ветки в другую нужно ввести команду:
 
    git merge <barnch_name>

где \<branch_name\> имя ветки, из которой будет производиться вливание изменений

## Удаление веток

Для удаления веток необходимо ввести команду:

    git brach -d <branch_name>

где \<branch_name\> имя ветки которую нужно удалить.

## Принудительное удаление ветор

Для принудительного удаления веток необходимо ввести команду 

    git branch -D <branch_name>

где \<branch_name\> имя ветки которую нужно удалить.

## Конфликные ситуации при слиянии веток

При возникновени конфликтных ситуации среда разработки даст вам подсказку о том как поступить в данной ситуации, вы можете выбрать изменения в ветке в которой находитесь или принять изменения из ветки слияни, так же вы можете принять все изменения, а потом уже поправить код так как вам нужно.

![Conflict situation](img\conflict.png)

## Удалённые репозиториип

Удалённые репозитории нужны для того чтобы вы могли делиться с коллегами своими разработками, а так же сами могли в любой момент подправить его, находясь за другим компьютером.


## **_THE END_**    
