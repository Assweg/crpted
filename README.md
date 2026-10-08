# crpted — Курсовая: веб-приложение с авторизацией (v1)

Курсовой проект, 4 семестр. Веб-приложение на Express + PostgreSQL: регистрация, вход, сессии, хеширование паролей.

## Что внутри
- `server.js` (~21К строк кода с маршрутами `/`, `/register`, `/home`)
- `db.js` — подключение к PostgreSQL через `pg`
- `import_data.js`, `data.js`, `data/` — загрузка тестовых данных
- `views/`, `public/` — страницы входа/регистрации
- `package.json`: express, pg, bcryptjs, express-session, body-parser, cors

## Стек
Node.js, Express 5, PostgreSQL, bcryptjs, express-session

## Запуск
```bash
npm install
node server.js
# по умолчанию порт 755
```

## Что изучено
Хеширование паролей, сессии, работа с PostgreSQL из Node.js, базовая защита форм.
См. также `crpted2` — вторая итерация с Docker.

---
**Автор:** Assweg · Telegram: [@assweg](https://t.me/assweg) · Учебное портфолио, все работы — студенческие.
