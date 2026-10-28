# Ход выполнения работ

## БЛОК 1

### 1 часть
1. Создала на GitHub репозиторий `infra-project`.
2. Склонировала его в VS Code через терминал.
3. Создала файл `.gitignore` и вписала туда три строки.
4. Запушила изменения на GitHub.

### 2 часть
1. Распаковала zip-папку.
2. Перетащила нужные папки/файлы в `infra-project`.
3. По очереди сделала три коммита.

### 3 часть
1. Второй `git diff` ничего не показал, потому что с помощью команды `git add` мы уже добавили содержимое файла в индекс (staged).

---

## БЛОК 2

### 1 часть

Вывод команды `git log --oneline`:
![alt text](image.png)

Вывод команды `git log --oneline --graph --all`:
![alt text](image-1.png)

Вывод команды `git show HEAD~1`:
![alt text](image-2.png)

**Текстовый вывод терминала:**
```bash
PS C:\Users\Lenovo\infra-project> git log --oneline --graph --all
* d165392 (HEAD -> main, origin/main) Отредактировать Readme.md
* 106bcd7 Сделать push папки ansible
* b030d24 Сделать push папки docker
* 7af8dc1 Сделать push .env.example и README.md
* 9e2fb72 Создать .gitignore

PS C:\Users\Lenovo\infra-project> git show HEAD~1
commit 106bcd7da621a31819486186abcab08a6b4e2659
Author: Zhanyl <bakirova_z@iuca.kg>
Date:   Wed Oct 28 22:31:41 2026 +0600

    Сделать push папки ansible
```

### 2 часть

Строка `HEALTHCHECK CMD wget -q0-http://localhost/ || exit 1`:
![alt text](image-5.png)

Вывод команды `git merge feature/healthcheck`:
![alt text](image-3.png)

Вывод команды `git branch -d feature/healthcheck`:
![alt text](image-4.png)

### 3 часть

Ошибка слияния (конфликт):
![alt text](image-6.png)

Вывод команды `git log --oneline --graph`:
![alt text](image-7.png)

Вывод команд `git pull` и `git log --oneline`:
![alt text](image-8.png)
