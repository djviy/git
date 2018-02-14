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
3. Коммит. Вводить -m обязательно(!) - комментарий коммита.
   ```
   git commit -m 'Добавлен файл file.txt'
   ```

**git add -i** - интерактивное добавление

## Убрать из коммита
**git reset path/to/file** переводит файл из состояния *staged* в *modified*  
**git checkout path/to/file** переводит файл из состояния *modified* в *unmodified* (команда сбрасывает изменения)

## История
**git log** - история коммитов
**$ git log -p** - diff всех изменений по коммитам (f и b - перемещаться по тексту)
**git show 3a64fcc** - просмотреть коммит *3a64fcc*
**git diff** - разница между репозиторием и рабочей копией (файлы со статусом *modified*) 




