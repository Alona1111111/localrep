# Початок роботи з GIT
- Завантажимо та інсталюємо https://git-scm.com/downloads
- Розглянемо основні команди для роботи з локальним репозиторієм

## Глобальна конфігурація GIT
- <code>git config --global user.name cameronmcnz</code>
- <code>git config --global user.email global-config@example.com</code>

## Файл .gitignore
- Вкажемо які файли не мають потрапити до VCS
- https://www.atlassian.com/ru/git/tutorials/saving-changes/gitignore

## Файл README.md
- Задокументуємо виконані операції 
- https://github.com/RichardLitt/standard-readme

## Ініціалізація репозиторія
<code>git init</code>

## Додаємо нові файли в коміт
- Вибірково <code>git add файл …</code>
- Всі нові <code>git add .</code>

## Перший коміт - фіксація змін
<code>git commit -m "Repo init"</code>

## Початок роботи з гілками
- Перелік гілок <code>git branch</code>
- Поточна гілка <code>git branch -v</code>
- Додамо всі нові зміни в індекс <code>git add .</code>
- Фіксація змін <code>git commit -m "Start work with branch"</code>

## Створення нової гілки
- Додамо нову гілку dev <code>git branch dev</code>
- Переглянемо перелік гілок <code>git branch</code>
- Перемкнемося на гілку dev <code>git checkout dev</code>

## Зливання гілки master з гілкою dev
- Перемкнемося на гілку master <code>git checkout master</code>
- Перевіримо статус змін гілки master <code>git status</code>
- Якщо гілка має не зафіксовані зміни їх потрібно завіксувати!
- Зливаємо гілку dev <code>git merge dev</code>
- Додамо всі нові зміни в індекс <code>git add .</code>
- Комітимо зміни <code>git commit -m "Merge master branch from dev"</code>

## Зливання гілки dev з гілкою master
- Перемкнемося на гілку dev <code>git checkout dev</code>
- Перевіримо статус змін гілки master <code>git status</code>
- Якщо гілка має не зафіксовані зміни їх потрібно завіксувати!
- Зливаємо гілку master <code>git merge master</code>
- Додамо всі нові зміни в індекс <code>git add .</code>
- Комітимо зміни <code>git commit -m "Merge dev branch from master"</code>

## Видалення гілки need_delete
- Створемо гілку для видалення <code>git branch need_delete</code>
- Видалимо гілку <code>git branch --delete need_delete</code>
- Додамо всі нові зміни в індекс <code>git add .</code>
- Комітимо зміни <code>git commit -m "Delete branch need_delete"</code>

## Створення конфлікт зливання гілок
- Додамо всі нові зміни в індекс <code>git add .</code>
- Комітимо зміни <code>git commit -m "Create merge conflict"</code>

## Вирішення конфлікти зливання гілок
Версія з гілки master
- строка конфликту зливання master dev
Версія з гілки dev
- строка конфликту  master dev зливання

# Відправлення до віддаленого репозиторію GitHub.com
- Додамо всі нові зміни в індекс <code>git add .</code>
- Комітимо зміни <code>git commit -m "Push to remote repository"</code>
- Відправка змін <code>git push origin master</code>