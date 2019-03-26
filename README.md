Устанавливаем VS Code
Устанавливаем https://git-scm.com программу
Перезапускаем ВСКод
открываем консоль ctrl + `
теперь нужно задать что настройки будут глобальные (можно и локальные но я не изучал как)
git config credential.helper store
git config --global user.name "jeromwork"
git config --global user.password "v0vy8l8fcygtmy6mn"
git config --global user.email "jeromwork@inbox.ru"
git config --global -e


git init

Если уже подключены к репозиторию отключаемся
git remote rm origin
Теперь подключаемся к выбранному репозиторию
git remote add origin https://github.com/jeromwork/test2.git
если что то не идет, ошибки, то можно посмотреть инфу на следующем сайте:
https://agladky.ru/blog/git-cheat-sheet/




файл 
.gitignore
#Игнорирует все в проекте кроме указаной папки как раз в той(!/wp_content/p/) где находится плагин и все изменения 
#но этот файл нужно создать сразу же и залить на сервер, т.к. он учитывает в своих правилах только те файлы
#которые были добавлены позже сохранения его правил
/*
!/wp_content/p/
.vscode
