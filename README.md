# Пример FastAPI + PostgreSQL

Простой проект. Сделан на фастапи и постгрес.  
Сохраняет пользователей и показывает их.

---

## Что тут используется

- fastapi — это фреймворк для апишек
- postgresql — база данных
- sqlalchemy — для работы с базой
- pydantic — для проверки данных

---

## Как запустить

git clone https://github.com/ТВОЙ_ЮЗЕРНЕЙМ/fastapi-postgres.git
cd fastapi-postgres


Создай виртуальное окружение

python -m venv venv
venv\Scripts\activate  # если Windows
# или
source venv/bin/activate  # если Linux или Mac


Установи зависимости

pip install -r requirements.txt
Сделай базу данных в PostgreSQL (например в pgAdmin или psql)



sql

CREATE DATABASE fastapidb;
ALTER USER postgres WITH PASSWORD '1234';
DATABASE_URL = "postgresql://postgres:1234@localhost/fastapidb"


Запусти сервер

uvicorn main:app --reload

http://127.0.0.1:8000/docs


Пример пользователя

{
  "name": "ASD",
  "email": "ASD@example.com"
}


