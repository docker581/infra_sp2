# infra_sp2
## Описание
Запуск docker-compose
## Команды
### Запуск приложения
docker-compose up -d
### Создание суперпользователя
docker-compose exec web python manage.py migrate --noinput
docker-compose exec web python manage.py createsuperuser
### Заполнение базы начальными данными
- В админке (localhost/admin)
- Через Postman (API)