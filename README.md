# git
Настройка и замечания по git

## Установка

- mac: brew install git
- ubuntu: sudo apt install git
- windows: choco install git

### Данные пользователя для коммитов
```
$ git config --global user.name "Vasily"
$ git config --global user.email "vasily@vasya.io"
```

## Инициализация
```
git init
```
После инициализации появляется поддиректория *.git*

### Скачивание (клонирование) репозитория себе в папку
```
git clone git@github.com:company-name/example.git
```

## Коммит
1. Проверяем состояние файлов (отслеживаются, добавлены, не добавлены)
   ```
   git status
   ```
2. Добавляются необходимые файлы для коммита (например *file.txt*)
   ```
   git add file.txt
   ```
3. Коммит. Ввобдить -m обязательно(!) - комментарий коммита.
   ```
   git commit -m 'Добавлен файл file.txt'
   ```
