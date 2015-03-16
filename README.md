#Github/git cheatsheet

##Форк и стягивание

1. Кнопка **Fork** в репозитории
2. **git clone** <адрес своего форка из поля справа>

##Коммиты

1. **git status** - просмотр состояния репозитория
2. **git add \<file\>** - добавление в stage; **git add .** - добавить всё
3. **git rm \<file\>** - staging удаления файла
4. **git commit -m "комментарий"** - коммит

##Отмена

1. **git reset HEAD \<file\>** - отмена внесения в stage (изменения перестают сопровождаться)
2. **git checkout -- \<file\>** - отмена изменений из unstaged файла

А как отменить коммит, спросите вы? А я вам отвечу: [идите нахуй!](http://www.youtube.com/watch?v=V1REMGv3_Ns)

##Быстрая правка коммита

**git commit --amend** - позволяет добавить изменения из stage в последний коммит (исправить его). Применять только в крайнем случае.

##Синхронизация форка

[Читать тут](https://help.github.com/articles/syncing-a-fork/)

##Отправка изменений

1. **git push** - отправить коммиты из локального репозитория в гитхабовский
2. **git pull** - наоборот, стянуть изменения из гитхаба в локальный репозиторий

##Ветки

 * **git branch \<name\>** - создать ветку
 * **git checkout \<name\>** - перейти на ветку
 * **git checkout -b \<name\>** - создать ветку и перейти в нее
 * **git merge \<другая ветка\>** - слияние: другая ветка мерджится в ту, в которой ты находишься
 
##Markdown

    #Заголовок 1 уровня
    ##Заголовок 2 уровня
    ######Заголовок 6 уровня
    *курсив*
    **жирный**
    [текст](http://example.com) - ссылка
    ![текст](http://example.com/1.jpg) - изображение
    4 пробела - код, неформатированный текст
    
     * маркированный список
     * еще пункт
     * * подпункт
     
    
    если пишешь не список, то текст, перенесенный
    на другую строку в результате будет в одной строке; для того, чтобы начать другую
    строку, нужно разделить два абзаца
    
    пустой строкой
    
если пишешь не список, то текст, перенесенный
на другую строку в результате будет в одной строке; для того, чтобы начать другую
строку, нужно разделить два абзаца
    
пустой строкой

##Прочее

**git init** - создать пустой репозиторий в этой папке (после этого все файлы в этой папке будут unstaged!)

##Самое главное

[Книга в формате pdf](https://github.com/downloads/GArik/progit/progit.ru.pdf)
[Второе издание на английском](https://github.com/progit/progit2/releases/download/2.0.0/progit-2.0.0.pdf)
