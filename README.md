# Учебная платформа по криптографии · первая итерация

![Стек](https://img.shields.io/badge/Node.js%20%C2%B7%20Express%20%C2%B7%20PostgreSQL-334155?style=flat-square) ![Семестр](https://img.shields.io/badge/семестр-4-0f766e?style=flat-square) ![Статус](https://img.shields.io/badge/статус-%D0%A3%D1%87%D0%B5%D0%B1%D0%BD%D1%8B%D0%B9%20%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82-64748b?style=flat-square)

Курсовой проект на Express и PostgreSQL: учётные записи, учебные материалы и тесты. Пароли обрабатываются с помощью bcryptjs, состояние входа хранится в сессии.

## Возможности и файлы

- [server.js](server.js) — Express-приложение, регистрация, вход и маршруты учебных материалов.
- [db.js](db.js) — подключение к PostgreSQL через переменные окружения.
- [views](views/) и [public](public/) — страницы и оформление.
- [data](data/), [import_data.js](import_data.js) — учебные материалы и их импорт.

## Подготовка

Нужны Node.js, npm и PostgreSQL. В `db.js` читаются `DB_HOST`, `DB_PORT`, `DB_USER`, `DB_PASSWORD`, `DB_NAME`. Задайте их в локальном `.env` и подготовьте схему БД. В этой версии нет отдельного SQL-файла инициализации; готовая схема есть в [следующей итерации](https://github.com/Assweg/crpted2/blob/main/db/init.sql).

## Запуск после настройки БД

```bash
npm ci
node import_data.js
node server.js
```

По умолчанию приложение использует порт `755`. Импорт требует уже созданных таблиц.

## Ограничения

Проект опубликован как учебная работа. Для воспроизводимого окружения с SQL-схемой и сервисом импорта удобнее начать со второй итерации.

## Версии

[Первая итерация](https://github.com/Assweg/crpted) · [Версия с Docker](https://github.com/Assweg/crpted2) · [Курсовые материалы](https://github.com/Assweg/crpted2).

---

[Каталог учебных репозиториев](https://github.com/Assweg/nstu) · [Профиль Assweg](https://github.com/Assweg)
