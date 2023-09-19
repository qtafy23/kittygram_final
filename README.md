# **Kittygram**


## **Описание**
Благодаря этому проекту можно будет публиковать и смотреть котиков в социальной сети.


### **Как запустить проект**

##### Клонировать репозиторий и перейти в него в командной строке:

```
git clone git@github.com:qtafy23/kittygram_final;

cd kittygram_final
```
##### Установить докер и запустить проект в контейнере

Инструкция по установке: [Docker](https://docs.docker.com/installation/mac/)

`docker compose -f docker-compose.production.yml up`

##### Выполнить миграции и собрать статику:

```
docker compose -f docker-compose.production.yml exec backend python manage.py migrate

docker compose -f docker-compose.production.yml exec backend python manage.py collectstatic

docker compose -f docker-compose.production.yml exec backend cp -r /app/collected_static/. /backend_static/static/
```


### Примеры запросов к API
```
GET http://127.0.0.1:8080/api/
```

```
POST http://127.0.0.1:8080/api/users/
```

```
POST http://127.0.0.1:8080/api/token/login/
```

```
POST http://127.0.0.1:8080/api/users/activation/
```

```
GET http://127.0.0.1:8080/api/cats/
```


### Автор
**Qtafy23**
