## git fetch

Для синхронизации текущей ветки с репозиторием используются команды *`git fetch`* и *`git pull`*.

**git fetch** — забирает изменения удаленной ветки из репозитория по умолчания, основной ветки; той, которая была использована при клонировании репозитория. Изменения обновят удаленную ветку (remote tracking branch), после чего надо будет провести слияние с локальной ветку командой *`git merge`*.

Получает изменений из определенного репозитория:

```bash=
git fetch /home/username/project
```

Возможно также использовать синонимы для адресов, создаваемые командой *`git remote`*:

```bash=
git remote add username-project /home/username/project
git fetch username-project
```

Естественно, что после оценки изменений, например, командой *`git diff`*, надо создать коммит слияния с основной:

```bash=
git merge username-project/master
```