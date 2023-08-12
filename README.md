## Работа с локальным репозиторием
- git init - Инициализировать репозиторий (иниуиализируется текущая папка)
- git status - Проверить статус или состояние репозитория 
- rm -rf .git - Разгитить папку (фактически, удалить из нее скрытую подпапку git, где хранятся служебные данные для гита)
- git add - добавить файлы которые потом будем коммитить
($ git add todo.txt или $ git add . или $ git add --all  # добавить всю текущую папку)
- git commit -m 'комментарий' - Выполнить коммит
- git log - Просмотреть историю коммитов


## Синхронизация с удаленным репозиторием
- создать на гитхабе удаленный репозиторий, взять на него ссылку (SSH)

- git remote add имя_удаленного_репозитория ссылка_на_удаленный_репозиторий - Привязать удалённый репозиторий к локальному
($ git remote add origin git@github.com:%ИМЯ_АККАУНТА%/first-project.git)

- git remote -v  - Убедиться, что репозитории связаны

- $ git push -u origin main - Отправить изменения на удалённый репозиторий. Флаг -u свяжет локальную ветку с одноимённой удалённой. Вдальнейшем его можно не использовать.