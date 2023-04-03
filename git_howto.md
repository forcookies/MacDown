# Подсказка по GIT

Создание репозитория
```sh
git init
```

Добавление нового файла
```sh
git add
```

Добавление поэтапных изменений файла
```sh
git commit -m "Message"
```

Просмотр истории изменений файла
```sh
git log
```

Обзор изменений файла в кратком виде
```sh
git log --oneline
```

Возврат к состоянию файла на определенном этапе
```sh
git checkout (тег совершенного изменения)
```

Возврат к текущему состоянию файла
```sh
git checkout master
```

Текущее состояние файла
```sh
git status
```

Просмотр изменений в коде файла
```sh
git diff
```

Добавление картинок
```sh
git add my-photo.png
```

Добавление имени пользователя
```sh
git config --global user.name "Ввести своё имя"
```

Добавление имейла пользователя
```sh
git config --global user.email "Ввести свой имейл"
```

Делаем fork репозитория, в которой потом хотим сделать pull request. Ищем кнопку fork на странице репозитория

Выполняем команду клонирования из своей fork-копии

git clone git@github.com:*YOURE_GITHUB*/version_control.git

Создаём новую ветку и вносим необходимые изменения в файл

git checkout -b updategit_howto
vim git_howto.md
git add git_howto.md
git commit -m "Добавили инструкцию как создать pull request"

Делаем push

git push --set-upstream origin updategit_howto

Переходим на свою страницу репозитория. Выбираем ветку updategit_howto и жмём кнопку Compare и pull request.