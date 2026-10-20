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

## Заказная разработка

### Memory Test

Разрабатывал backend веб-приложения для тренировки памяти и когнитивных функций пользователей старшего возраста. Работал в команде из 22 человек (6 frontend-разработчиков, 6 backend-разработчиков, 9 дизайнеров, менеджер).
В команде backend-разработчиков я отвечал за следующие задачи:
* настройка проекта;
* поддерживал документацию OpenAPI;
* реализовал функционал задач тренажера на ввод ответов;
* реализовал функционал задач на связывание пар ответов;
* реализовал функционал задач c группировкой ответов;
* реализовал multi stage build в Docker;
* код-ревью реализации бизнес‑логики
* отвечал за слияние feature‑ и hotfix‑веток в develop: проводил финальную проверку коммитов, разрешал конфликты слияния;
* дорабатывал код по замечаниям тимлида;
* согласовывал с фронтенд‑командой приоритеты багов и сроки их устранения.

*В проекте используется следующий стек*
* Python
* Django (DRF)
* PostgreSQL
* Docker
* Pytest
* OpenAPI.

**Deadline** - *60 дней*. **Время выполнения** - *60 дней*.

## Backend-сервисы

1) ### [Deribit Price Service](https://github.com/Andrey-Dubov-25/deribit-price-service)

Реализовал асинхронный клиент Deribit на aiohttp с retry и обработкой
ошибок. Настроил периодический сбор цен через Celery Beat + Worker
с сохранением в PostgreSQL. Разработал REST API на FastAPI: три
GET-метода с валидацией параметров и Swagger-документацией. Спроектировал
схему БД с составным индексом под все запросы API; миграции Alembic.
Написал 5 unit-тестов (pytest + aioresponses + AsyncMock). Подготовил
Docker Compose из 5 сервисов с healthcheck'ами и автонакатом миграций.
Настроил ruff и описал архитектурные решения в README.

*В проекте используется следующий стек*
* Python
* FastAPI
* SQLAlchemy (async)
* Alembic
* Celery
* Redis
* aiohttp
* PostgreSQL
* Docker
* Pytest
* Ruff
  
**Deadline** - *3 дня*. **Время выполнения** - *2 дня*.

2) ### [Guild Quest Board](https://github.com/Andrey-Dubov-25/guild_quest_board)
  
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

3) ### [Grocery Store](https://github.com/Andrey-Dubov-25/grocery_store)
  
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

4) ### [Booking](https://github.com/Andrey-Dubov-25/booking)
   
Реализовал API тестовой страницы сервиса бронирования, на которой пользователь получает информацию о дальнейших шагах (с помощью ИИ) при заселении в отель.

*В проекте используется следующий стек*
* Python
* FastAPI
* Groq

**Deadline** - *1 день*. **Время выполнения** - *6 часов*.
    
5) ### [Departments](https://github.com/Andrey-Dubov-25/departments)
  
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

6) ### [MyLibrary](https://github.com/Andrey-Dubov-25/my_library)
   
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
