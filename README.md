# **Kittygram**


## **Описание**
Благодаря этому проекту можно будет публиковать и смотреть котиков в социальной сети.


### **Как запустить проект**

##### Клонировать репозиторий и перейти в него в командной строке:

```
git clone git@github.com:qtafy23/kittygram_final;

cd kittygram_final
```
##### Cоздать и активировать виртуальное окружение:

`cd backend`
`python3 -m venv venv`
`source venv/bin/activate`

##### Установить зависимости из файла requirements.txt:

`python -m pip install --upgrade pip`
`pip install -r requirements.txt`

##### Выполнить миграции:

`python manage.py migrate`

##### Запустить проект:

`python manage.py runserver`


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
