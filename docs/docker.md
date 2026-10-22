# Запуск в Docker

## Сборка образа

```bash
docker build -t cloud-team-app:v1 .
```

## Запуск контейнера

```bash
docker run -d --name cloud-team-app -p 8080:5000 cloud-team-app:v1
```

## Порты

| Где | Порт | Зачем |
|-----|------|-------|
| Внутри контейнера | 5000 | на нем слушает Flask |
| На хосте | 8080 | сюда заходим из браузера или curl |

Флаг `-p 8080:5000` перенаправляет запросы с 8080 хоста на 5000 контейнера.

## Переменные окружения

Настройки передаются при запуске через `--env-file`, пример файла лежит в `config/example.env`:

```bash
docker run -d --name cloud-team-app -p 8080:5000 --env-file config/.env cloud-team-app:v1
```

## Проверка

```bash
docker ps
curl http://localhost:8080
```
