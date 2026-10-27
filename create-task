# Create task

##Actor
Клиент (Браузер)

##Predictions
Должны совпадать: дата и время...

##Main flow
1) Запрос от клиента на создание/изменение базы данных:
(```http
POST /tasks HTTP/1.1
Host: UTT.example.com
Content-Type: application/json
```
```json
{
  "title": "Лабораторная работа № 1",
  "status": "in_progress",
}
```)

2) Проверка и применение изменений/ответ, запрашиваемый клиентом

3)Ответ сервера запрос клиента:
(```http
HTTP/1.1 201 ACCEPTED
Content-Type: application/json
```
```json
{
  "id": "271"
  "title": "Лабораторная работа № 1",
  "status": "in_progress",
}
```)

## Alternative flows
### Empty title
При пустом названии, сервер:
1) Возвращает ошибку, а интерфейс просит клиента задать название
2) Автоматически даёт объекту (работе/заданию) имя "Untitled #N"

