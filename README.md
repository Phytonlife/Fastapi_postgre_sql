# 🚀 Пример FastAPI + PostgreSQL + Docker

Простой проект API на FastAPI с базой PostgreSQL.  
Можно сохранять пользователей и получать их список.  
Подходит как старт для своих проектов.

---

## 🧰 Что используется

- **FastAPI** — современный фреймворк для создания API
- **PostgreSQL** — база данных
- **SQLAlchemy** — работа с базой через Python
- **Pydantic** — проверка данных
- **Docker** — чтобы не настраивать всё вручную

---

## 📦 Как запустить в Docker (рекомендуется)

> Работает сразу, без установки Python и базы.

1. Убедись, что установлен [Docker Desktop](https://www.docker.com/products/docker-desktop/)

2. Склонируй репозиторий:


git clone https://github.com/ТВОЙ_ЮЗЕРНЕЙМ/fastapi-postgres.git
cd fastapi-postgres


## Запусти проект

Редактировать
docker-compose up --build

Документация Swagger: http://localhost:8000/docs

## Структура проекта

fastapi-postgres/
│
├── main.py               # основной файл приложения
├── models.py             # модель базы данных
├── schemas.py            # схемы Pydantic
├── crud.py               # функции для работы с БД
├── database.py           # подключение к базе
├── Dockerfile            # инструкция как собрать контейнер
├── docker-compose.yml    # как запустить сразу и бэкенд, и БД
├── requirements.txt      # зависимости Python
└── README.md       