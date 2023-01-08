# Репозиторий первого модуля работы с Git
[Git Logo](https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png)

## Описание репозитория 

Зачем была создана система контроля версий Git? 
> **_Torvalds_**: I really never wanted to do source control management at all and felt that it was just about the least interesting thing in the computing world (with the possible exception of databases ;^), and I hated all SCM’s with a passion. But then BitKeeper came along and really changed the way I viewed source control. BK got most things right and having a local copy of the repository and distributed merging was a big deal. _The big thing about distributed source control is that it makes one of the main issues with SCM’s go away – the politics around “who can make changes.” BK showed that you can avoid that by just giving everybody their own source repository_. But BK had its own problems, too; there were a few technical choices that caused problems (renames were painful), but the biggest downside was the fact that since it wasn’t open source, there was a lot of people who didn’t want to use it. So while we ended up having several core maintainers use BK – it was free to use for open source projects – it never got ubiquitous. So it helped kernel development, but there were still pain points.

### Процесс создания git-репозитория для локальной работы в общем случае выглядит так:

```
git init
git checkout -b feature-branch
git remote add origin "ssh@myremote.com/repo.git"
touch .gitignore 
git add . 
git commit -m "Initial comit"
git push
```
### Чтобы работать с другой учетной записью git локально, можно в глобальный конфиг .gitconfig добавить строки:  
```
[includeIf "gitdir:~/rebrain/"]
    path = ~/rebrain/.gitconfig
[init]
	defaultBranch = main
```
Далее при работе в папке "~/rebrain/\*" будет использоваться указанный в ней файл .gitconfig (вместо глобального конфига), содержащий email и name другой учетной записи (и другие параметры конфигурации git по необходимости)

### На момент выполнения задания GIT 04 в репозитории находятся два файла:
1. README.md  : файл с описанием репозитория в языке разметки markdown
	- Файлы REAMDE содержат информацию, необходимую для ознакомления и работы с репозиторием
2. nginx.conf : файл стандартной конфигурации nginx
	- Файл nginx.conf содержит конфигурацию, определяющую количество рабочих процессов и поведение (работу) сервера Nginx

### Taблица со статусом выполнения заданий первого модуля:

| Код Задания | Статус Выполнения |
| ----------- | ----------- |
| GIT-01      | Выполнено   |
| GIT-02      | Выполнено   |
| GIT-03      | Выполнено   |
| GIT-04      | Выполняется |
| GIT-05      | Не Выполнено|
| GIT-06      | Не Выполнено|
| GIT-07      | Не Выполнено|
| GIT-08      | Не Выполнено|
| GIT-09      | Не Выполнено|
| GIT-10      | Не Выполнено|
| GIT-11      | Не Выполнено|
| GIT-12      | Не Выполнено|
| GIT-13      | Не Выполнено|
| GIT-14      | Не Выполнено|
| GIT-15      | Не Выполнено|
| GIT-16      | Не Выполнено|
