# 📊 Телеграм-бот "Финансовый помощник"

Бот для учета личных финансов, отслеживания курса валют и получения советов по экономии.

## 🚀 Возможности

- **Регистрация пользователей** в системе
- **Курсы валют** (USD/RUB, EUR/RUB) через API
- **Советы по экономии** (рандомные полезные советы)
- **Учет расходов** по 3 категориям
- **Сохранение данных** в SQLite базу

## 🛠 Технологии

- Python 3.11+
- Aiogram 3.x (асинхронный фреймворк)
- SQLite3 (хранение данных)
- ExchangeRate-API (курсы валют)

## ⚙️ Установка

1. Клонировать репозиторий:
   ```bash
   git clone https://github.com/ваш-репозиторий/finance-bot.git
   cd finance-bot
2. Установить зависимости:

   pip install -r requirements.txt

3. Создать файл config.py с вашим токеном:
   TOKEN = "ваш_токен_бота"
4. Запустить бота:
   python main.py

## 📌 Команды
   /start - запуск бота


## 📈 База данных
   Структура таблицы users:

   CREATE TABLE users (
      id INTEGER PRIMARY KEY,
      telegram_id INTEGER UNIQUE,
      name TEXT,
      category1 TEXT,
      category2 TEXT,
      category3 TEXT,
      expenses1 REAL,
      expenses2 REAL,
      expenses3 REAL
   )
