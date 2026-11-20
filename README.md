# Седьмая работа по предмету

Цель: доработка task3, включающая в себя переписывание интерфейса с CLI до Web UI

Использован Flask

## Запуск, остановка, использование

Запуск
```
sh tools/deploy.sh
```

Пример настройки в .env (заменяется tools/gen-env.sh)
```
POSTGRES_USER=pgowner
POSTGRES_PASSWORD=<заменяется автоматически>
POSTGRES_DB=standoff
JUDGE_USER=judge
JUDGE_PASSWORD=<заменяется автоматически>
LOCAL_UID=<uid>
LOCAL_GID=<gid>
WEB_PORT=<порт>
```

Веб-сервис поднимется на 8077 по умолчанию

Остановка
```
docker compose down -v
```

## Пояснение к .env, секретам
В репозитории указаны демонстрационные пароли/секреты
Перед использованием нужно сгенерировать .env с помощью tools/gen-env.sh