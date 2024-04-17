Для проверки функциональности эндпоинтов в Postman, следует отправить запросы на соответствующие URL-адреса с учетом типа запроса (GET, POST, PUT, PATCH, DELETE) и ожидаемых данных.

Вот какие запросы можно отправить для каждого из эндпоинтов:

1. Список курсов (GET):
URL: http://127.0.0.1:8000/courses/
Тип запроса: GET

2.Получение курса по идентификатору (GET):
URL: http://127.0.0.1:8000/courses/<course_id>/
Тип запроса: GET
<course_id> - идентификатор курса, который нужно получить

3.Создание курса (POST):
URL: http://127.0.0.1:8000/courses/create/
Тип запроса: POST
Тело запроса должно содержать данные нового курса в формате JSON, например:
json
{
    "title": "Название курса",
    "description": "Описание курса"
}

4.Обновление курса (PUT или PATCH):
URL: http://127.0.0.1:8000/courses/<course_id>/update/
Тип запроса: PUT или PATCH
<course_id> - идентификатор курса, который нужно обновить
Тело запроса должно содержать обновленные данные курса в формате JSON

5.Удаление курса (DELETE):
URL: http://127.0.0.1:8000/courses/<course_id>/delete/
Тип запроса: DELETE
<course_id> - идентификатор курса, который нужно удалить
Аналогично, для эндпоинтов уроков:

1.Список уроков (GET):
URL: http://127.0.0.1:8000/lessons/
Тип запроса: GET

2.Получение урока по идентификатору (GET):
URL: http://127.0.0.1:8000/lessons/<lesson_id>/
Тип запроса: GET
<lesson_id> - идентификатор урока, который нужно получить

3.Создание урока (POST):
URL: http://127.0.0.1:8000/lessons/create/
Тип запроса: POST
Тело запроса должно содержать данные нового урока в формате JSON

4.Обновление урока (PUT или PATCH):
URL: http://127.0.0.1:8000/lessons/<lesson_id>/update/
Тип запроса: PUT или PATCH
<lesson_id> - идентификатор урока, который нужно обновить
Тело запроса должно содержать обновленные данные урока в формате JSON

5.Удаление урока (DELETE):
URL: http://127.0.0.1:8000/lessons/<lesson_id>/delete/
Тип запроса: DELETE
<lesson_id> - идентификатор урока, который нужно удалить