# Портфолио backend-разработчика (Python)

## Pet-проекты

### [МФК «Восход»](https://github.com/Andrey-Dubov-25/futsal_team)

Разрабатываю сайт для реальной любительской мини-футбольной команды
из Владимира. Проект включает публичный сайт, REST API, парсер данных
с сайта городской Лиги (befutsal.ru) и prod-инфраструктуру.

Реализовал 12 моделей (игроки, матчи, события, новости, комментарии,
тренеры, тренировки, фотоальбомы, турниры), REST API с JWT-авторизацией,
фильтрацией, поиском, сортировкой и пагинацией; документация через
Swagger. Разработал парсер внешнего источника с management-командой
`sync_befutsal` — данные с Лиги (турниры, места, общая статистика)
синхронизируются автоматически. Написал 259 тестов (pytest + factory-boy)
с моками внешних API. Настроил CI/CD на GitHub Actions: линтеры,
тесты, проверка форматирования на каждый push. Подготовил prod-конфиг
с Docker Compose, Nginx, Gunicorn и collectstatic. Фронтенд — Django
Templates + HTMX: 12+ страниц, тёмная/светлая тема, SEO, мобильная
адаптивность, галерея с лайтбоксом.

*В проекте используется следующий стек*
* Python
* Django
* DRF
* Pytest
* PostgreSQL
* Docker
* Nginx
* Gunicorn
* HTMX
* GitHub Actions
* Ruff

**Статус** — *активно развивается*.


## Backend-сервисы
1) [GQB](https://github.com/Andrey-Dubov-25/guild_quest_board)
  
Разработал backend‑сервис для доски квестов фэнтези‑гильдии на Django + DRF с использованием PostgreSQL. Настроил запуск через Docker Compose, подготовил документацию API (Redoc), README с подробной инструкцией по развёртыванию и тесты для основных бизнес‑процессов. Проект готов к интеграции с фронтендом и масштабированию.

*В проекте используется следующий стек*
* Python
* Django
* DRF
* Pytest
* PostgreSQL
* Docker
* Redoc
  
**Deadline** - *1 неделя*. **Время выполнения** - *5 дней*.

2) [Grocery Store](https://github.com/Andrey-Dubov-25/grocery_store)
  
Разработал backend‑сервис для продуктового магазина на Django + DRF с использованием PostgreSQL. Настроил запуск через Docker Compose, подготовил документацию API (Swagger), README с подробной инструкцией по развёртыванию и тесты для основных бизнес‑процессов. Проект готов к интеграции с фронтендом и масштабированию.

*В проекте используется следующий стек*
* Python
* Django
* DRF
* Pytest
* PostgreSQL
* Docker
* Redoc
  
**Deadline** - *1 неделя*. **Время выполнения** - *3 дней*.

3) [Booking](https://github.com/Andrey-Dubov-25/booking)
   
Реализовал API тестовой страницы сервиса бронирования, на которой пользователь получает информацию о дальнейших шагах (с помощью ИИ) при заселении в отель.

*В проекте используется следующий стек*
* Python
* FastAPI
* Groq

**Deadline** - *1 день*. **Время выполнения** - *6 часов*.
    
4) [Departments](https://github.com/Andrey-Dubov-25/departments)
  
Реализовал API для управления подразделениями и сотрудниками с защитой от циклических ссылок, каскадным удалением и получением дерева подразделений заданной глубины. Использовал рекурсивный подход для построения иерархии.

*В проекте используется следующий стек*
* Python
* Django
* DRF
* Pytest
* PostgreSQL
* Docker
* Redoc

**Deadline** - *1 неделя*. **Время выполнения** - *4 дня*.

5) [YaCut](https://github.com/Andrey-Dubov-25/async-yacut)

Разработал Flask‑приложение с асинхронным взаимодействием с внешним API — пользователь загружает оригинальный вариант ссылки на какой-либо сайт или файл со своего устройства и получает вариант короткой ссылки, при переходе по которой открывается оригинальный вариант ссылки или файла.

*В проекте используется следующий стек*
* Python
* Flask
* aiohttp
  
**Deadline** - *2 недели*. **Время выполнения** - *1 недели*.

6) [MyLibrary](https://github.com/Andrey-Dubov-25/my_library)
   
Разработал REST API для управления списком книг.  Приложение умеет добавлять книги, показывать список, искать конкретную книгу, обновлять данные и удалять книги.

*В проекте используется следующий стек*
* Python
* FastAPI
* SQLAlchemy
* aiosqlite

**Время выполнения** - *5 дней*

## Сертификаты
* [Яндекс.Практикум - python-разработчик](https://github.com/Andrey-Dubov-25/Practicum_projects/blob/main/сertificates/yandex_practicum.jpg)
* [Stepic - Python для начинающих](https://github.com/Andrey-Dubov-25/Practicum_projects/blob/main/сertificates/stepic_beginner.jpg)
* [Stepic - Python для продвинутых](https://github.com/Andrey-Dubov-25/Practicum_projects/blob/main/сertificates/stepic_advanced.jpg)
* [Stepic - ООП-база](https://github.com/Andrey-Dubov-25/portfolio/blob/main/сertificates/ООП-база.jpg)
* [Stepic - ООП-продвинутый](https://github.com/Andrey-Dubov-25/portfolio/blob/main/сertificates/ООП-продвинутый.jpg)
