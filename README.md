<div align="center">

  <h3>RUD3US</h3>

<img
    src="https://avatars.githubusercontent.com/u/80245370?v=4"
    alt="Rudy Icon"
    width="180"
    style="border-radius: 50%; box-shadow: 0 8px 24px rgba(0,0,0,0.18); border: 1px solid #e5e7eb;"
  />

  <p><sub>Used Services:</sub></p>

</div>

<p align="center">
  <a href="https://github.com/RudySource?tab=repositories">
    <img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
  <a href="https://dotnet.microsoft.com/">
    <img src="https://img.shields.io/badge/.NET-5C2D91.svg?style=for-the-badge&logo=.net&logoColor=white"/>
  </a>
  <a href="https://www.sqlite.org/">
    <img src="https://img.shields.io/badge/SQLite-003B57.svg?style=for-the-badge&logo=sqlite&logoColor=white"/>
  </a>
  <a href="https://learn.microsoft.com/dotnet/csharp/">
    <img src="https://img.shields.io/badge/C%23-239120.svg?style=for-the-badge&logo=c-sharp&logoColor=white"/>
  </a>
</p>

<div align="center" style="max-width: 600px; margin: 0 auto; padding: 18px; border-radius: 18px; background: rgba(255,255,255,0.06); box-shadow: 0 14px 30px rgba(0,0,0,0.08);">

## Основная информация

**ФИО**: Rudy Rudy Rudy

**Группа**: ИСП-233

**Дата**: 24.08.2077

</div>

# Лабораторная работа №36. Итоговый проект: TaskBoard

## Описание проекта

`TaskBoard` - это небольшое fullstack-приложение для управления списком задач. Проект состоит из двух частей:

- backend на `ASP.NET Core Web API`;
- frontend на `HTML`, `CSS` и `JavaScript`;
- база данных `SQLite`, подключенная через `Entity Framework Core`.

# Что мы строим

**TaskBoard** - это интерактивная доска задач. Приложение позволит пользователю:

- Просматривать актуальный список задач.
- Добавлять новые задачи (название + описание).
- Менять статус: отмечать задачу как выполненную (она визуально перечёркивается).
- Редактировать: изменять текст задачи прямо в интерфейсе.
- Удалять ненужные записи.

---

## Краткая инструкция по запуску

### 1. Запуск backend

Откройте терминал в папке `TaskBoardApi` и выполните:

```bash
dotnet run
```

После запуска API будет доступен по адресу:

```text
http://localhost:5085
```

Swagger в режиме разработки:

```text
http://localhost:5085/swagger
```

### 2. Открытие frontend

Откройте в браузере файл:

```text
frontend/index.html
```

Фронтенд отправляет запросы в API по адресу:

```text
http://localhost:5085/api/tasks
```

> [!WARNING]
> Важно: frontend нужно открывать после запуска backend, иначе список задач не загрузится.

---

## Главные выводы

1. Я закрепил, как frontend и backend взаимодействуют друг с другом через HTTP-запросы.
2. Я увидел, что `ASP.NET Core Web API` позволяет быстро создать сервер с готовыми маршрутами для CRUD-операций.
3. Я понял, как `Entity Framework Core` упрощает работу с базой данных и миграциями.
4. Я убедился, что даже простой frontend на чистом JavaScript может полноценно работать с API без дополнительных библиотек.
5. Я понял, насколько важно согласовать адреса и порты между клиентской и серверной частью приложения.
6. Я закрепил навык разделения проекта на независимые части: интерфейс, серверную логику и хранение данных.

> [!TIP]
> А если реал, я научился связывать back & front, как работает back с сайтом и http запросы, и то, что нужно проверять установенные библиотеки - их версии!
