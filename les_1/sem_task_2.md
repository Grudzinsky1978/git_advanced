# Задание 2

* Создать связь с репозиторием 1 `git remote add source [path]` (название другое - source)
* Просмотреть связи `git remote -v`
* Внести изменения в локальный код, добавить файл, изменить README.md, закоммитить, потом отправить изменения
```
git push -u origin main
git push -u source main
```
* Просмотреть изменения, зайти в удалённые репозитории на сайте
* Внести изменения в удалённых репозиториях (в обоих)
* Затянуть изменения `git fetch --all`
* Просмотреть изменения
```
git log origin/main ^main
git log source/main ^main
```
* Слить изменения с веткой main
```
git merge origin/main
git merge source/main
```

---

```
git remote add source https://github.com/Grudzinsky1978/remote-test-1.git
git remote -v
origin  https://github.com/Grudzinsky1978/remote-test-2.git (fetch)
origin  https://github.com/Grudzinsky1978/remote-test-2.git (push)
source  https://github.com/Grudzinsky1978/remote-test-1.git (fetch)
source  https://github.com/Grudzinsky1978/remote-test-1.git (push)
```
Изменил README.md
```
git status
git add .
git commit -m "README.md has been changed"
git push -u origin main
git push -u source main
```
Вижу изменения в обоих удалённых репозиториях

Внёс изменения в удалённые репозитории. В первом репозитории добавлен файл index.html, во втором изменён файл REAME.md.
```
git fetch --all
```
Изменения есть, но они не слиты
```
ll
```
Ещё нет нового файла index.html

Просмотр изменений
```
git log origin/main ^main
git log source/main ^main
```

Вливаю в текущую ветку
```
git merge origin/main
git merge source/main
```
Во втором случае редактор предложил сообщение коммита, которое надо подтвердить, нажав на галочку вверху справа в Visual Studio Code
```
git log --oneline
git push
```