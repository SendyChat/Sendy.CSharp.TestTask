# Library API 🏛️

Web API для управления библиотекой книг и авторов на .NET 8+

## Требования

* .NET 8+
* ASP.NET Core Web API
* Entity Framework Core (Code-First, миграции)
* AutoMapper
* Serilog
* Swagger / OpenAPI
* Custom middleware
* Глобальная обработка ошибок (ProblemDetails)
* Валидация DTO
* DI (встроенный контейнер ASP.NET Core)

## Задачи

1. ✨ Спроектировать модели `Author` и `Book`.
2. 🚀 Настроить EF Core:

   * Создать `DbContext`.
   * Добавить миграции.
   * Реализовать seeder для начальных данных.
3. 🔄 Настроить AutoMapper для маппинга Entity ↔ DTO.
4. 📦 Реализовать CRUD-эндпоинты:

   * GET (список и по id).
   * POST.
   * PUT.
   * DELETE.
5. 🛡️ Добавить middleware:

   * `TimingMiddleware` — логирование времени запросов.
   * `ApiKeyMiddleware` — проверка заголовка `X-Api-Key`.
6. 📝 Настроить Serilog (консоль + файл с роллингом по дате).
7. 🌐 Подключить Swagger / OpenAPI.
8. 🚨 Реализовать глобальную обработку ошибок (возврат `ProblemDetails`).
9. ✅ Добавить валидацию DTO (DataAnnotations или FluentValidation).

## Критерии оценки

* Корректность CRUD-операций.
* Чистота архитектуры и разделение ответственности.
* Правильная работа EF Core (миграции, seeder).
* Настройка AutoMapper и валидация DTO.
* Работа middleware и логирование.
* Наличие и корректность документации Swagger.
* Читабельность кода и структура репозитория.
* (Опционально) Unit-тесты или Dockerfile.
