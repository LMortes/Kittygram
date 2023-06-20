### Kittygram — социальная сеть для обмена фотографиями любимых питомцев. 

### Как запустить проект:
Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/LMortes/kittygram_final.git
```

```
cd kittygram_final
```
## Как запустить проект
Запустить проект командой:

```
docker compose up
```
## В другом терминале:

Применить миграции для базы данных, собрать статику бэкенда:

```
docker compose exec backend python manage.py migrate
```
```
docker compose exec backend python manage.py collectstatic
```
```
docker compose exec backend cp -r /app/collected_static/. /static/static/
```

## Перейти по адресу:
http://127.0.0.1:9000
или
http://localhost:9000

