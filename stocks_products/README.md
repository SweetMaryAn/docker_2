# Команды


Собрать образ:

```bash
docker build .
```
Создать контейнер:

```bash
docker run -d -p 7777:8000 "идентификатор образа"
```
Проверяем работоспособность API:

```bash
POST http://localhost:7777/api/v1/products/
Content-Type: application/json

{
    "title": "aple1",
    "description": "beautiful11"
}

GET http://localhost:7777/api/v1/products/
```
