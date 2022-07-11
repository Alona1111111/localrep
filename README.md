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

