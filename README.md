# Cloud Team Project

Учебный проект по дисциплине «Основы облачных технологий».
Вариант 4 – проект контейнерного приложения.

## Команда и роли

- Nepreff – владелец репозитория, разработчик, reviewer

## Выполненные задачи

| Issue | Что сделано | Ветка | Pull Request |
|-------|-------------|-------|--------------|
| #1 Создать структуру проекта | каталоги app, docs, config, простое Flask-приложение | feature/project-structure | #4 |
| #2 Документация Docker | Dockerfile и docs/docker.md с инструкцией запуска | feature/docker-docs | #5 |
| #3 Файл конфигурации | config/example.env без секретов, .gitignore | feature/config-example | #6 |

## Структура

```
cloud-team-project/
├── app/
│   ├── app.py
│   └── requirements.txt
├── config/
│   ├── README.md
│   └── example.env
├── docs/
│   ├── README.md
│   └── docker.md
├── .gitignore
├── Dockerfile
└── README.md
```

## Как работали

Каждая задача заведена как Issue, под нее сделана отдельная ветка, изменения попадали в main только через Pull Request после проверки.
