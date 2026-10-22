# Запуск в Docker

## Сборка образа

```bash
docker build -t cloud-team-app:v1 .
```

## Запуск контейнера

```bash
docker run -d --name cloud-team-app -p 8080:5000 cloud-team-app:v1
```

## Проверка

```bash
docker ps
curl http://localhost:8080
```
