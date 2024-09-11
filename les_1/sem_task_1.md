# Задание 1
* Создайте удалённый репозиторий remote-test-1 с файлом README.md
* Склонируйте его на свой рабочий стол `git clone`
* Посмотрите связи с удалённым репозиторием `git remote -v`
* Создайте новый **пустой** удалённый репозиторий remote-test-2
* Удалите связь с текущем репозиторием `git remote remove origin`
* Подключите свой локальный репозиторий к новому удалённому `git remote add origin` [path]
* Отправьте изменения в новый удалённый репозиторий `git push -u origin master (main)`

---

В терминале. Перешёл в папку рабочего стола:
```
cd [path]
```

Создал удалённый репозиторий 1, отметил чекбокс для создания README.md

```
git clone https://github.com/Grudzinsky1978/remote-test-1.git
git remote -v
```

Создал удалённый репозиторий 2, не отмечал чекбокс для создания README.md

```
git remote remove origin
git remote add origin https://github.com/Grudzinsky1978/remote-test-2.git
git remote -v
git push -u origin main
```

## PS
В видео семинара последняя команда указывала на master. Надо было заменить на main