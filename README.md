# Шпаргалка по git

## Создание репозитория в текущем каталоге:
```
git init
```
## Клонирование репозитория:
```
git clone <repository>
```
например:
```
git clone https://github.com/git/git.git
```
## Определение состояния файлов:
```
git status
```
## Отслеживать новые файлы (добавить в индекс)
```
git add [<pathspec>...]
```
например:
```
git add .
```
добавить в индекс все файлы в текущем каталоге и всех его подкаталогах.


# Создание команды git hist — красивый лог коммитов
Для того, чтобы каждый раз не вводить длинные команды для отображения истории коммитов git, сделаем алиас:
```
git config --global alias.hist "log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit"
```
