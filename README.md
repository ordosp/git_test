Небольшая инструкция по работе с Git.

## Создание нового локального репозитория
Нужно перейти в нужный каталог и ввести:
```bash
git init
```

## Добавление коммита
```bash
# git add <file> or
git add --all

git commit -m "First commit"
```

## Просмотр истории коммитов
```bash

# в полном виде
git log

# в сокращенном виде
git log --oneline
```

HEAD - последний (самый новый) коммит.


## Схема
```mermaid
graph LR;
  untracked -- "git add"    --> staged;
  staged    -- "git commit" --> tracked/comitted;
```

## Исправить последний коммит
Работает только с последним коммитом (HEAD).
```bash
git add <что-то>
git commit --amend --no-edit
```
