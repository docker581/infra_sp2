# infra_sp2

## Описание проекта
Разворачивание проекта (блог с API) в 3 docker-контейнерах

## Стек технологий
- Python 3.8.5
- Django 3.0.5
- Django Rest Framework (DRF) 3.11.0
- Docker-compose 3.3
- Postgres 12.4
- Nginx 1.19.3

## Установка docker
https://docs.docker.com/engine/install/

## Команды
### Клонирование репозитория
```
git clone https://github.com/docker581/infra_sp2
```

### Запуск приложения
```
docker-compose up -d
```

### Создание суперпользователя
```
docker-compose exec web python manage.py migrate --noinput
```
```
docker-compose exec web python manage.py createsuperuser
```

### Заполнение базы начальными данными
- В админке (localhost/admin/)
- С помощью готового набора данных
```
python3 manage.py loaddata fixtures.json
```

## Автор
Докторов Денис, студент факультета Бэкенд Яндекс Практикум