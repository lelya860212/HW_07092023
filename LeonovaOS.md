# *Инструкция по использованию системы контроля версий Git*
## Представляемся системе контроля версий
*Перед первым использованием, необходимо представиться.*
* git config --global user.email "you@example.com"
* git config --global user.name "Your Name"
## Инициализация локального репозитория
*Репозиторий - это хранилище файлов, поддерживающее версионность*
* git init 
## Информация о текущем состоянии Git
* git status
## Добавление файла
* git add Имя файла.расширение
## Создание коммита
*Коммит - это фиксация изменений и появление новой версии файла*
Перед сохранением необходимо сохранить версию файла и добавить его в репозиторий командой git add  Имя файла с расширением
* git commit -m "Коментарий"
## Вывод на экран всей истории коммитов
*Коммиты выводяться в хронологической последовательности*
* git log
*Для выхода из просмотра истории необходимо нажать q*
## Переход от одного коммита к другому
* git checkout
## Возвращение к актуальному состоянию
* git checkout master
## Разница между текущим файлом и последним закоммиченным
* git diff
# Работа с новыми ветками в Git
## Создание новой ветки
* git branch
## Слияние веток 
* git merge <Название ветки>
## Решение конфликтов
При работе в двух ветках одновременно может
возникнуть ситуация, когда в одной и другой
ветке мы по-разному изменили блок текста.
Если затем мы попробуем слить эти ветки, Git
сообщит о конфликте и предложит выбрать,
какие же изменения записать. 
![Конфликт версий](Конфликт.png)
## Визуализация всех веток
*git log --graph