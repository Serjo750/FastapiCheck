# Приложение для обработки запросов
## Запуск контейнера
Для запуска контейнера вам необходимо выполнить:
```sh
docker-compose up --build
```
--------------------------------
Адрес для подключение к запущенному приложению:

```sh
http://localhost:8008/docs#/default/get_table_info_selected_get
```
--------------------------------
## Функционал
При переходе по указанному выше адресу можно найти 2 поля
- '/'
- '/selected'

В поле  question_num в разделе / следует указать количество вопросов,
которые будут записаны в таблицу базы данных со следующими полями:
- id
- question
- answer
- created_at
-------------------------------
В разделе '/selected' при получении GET запроса выводится результат выполнения select запроса таблицы базы данных по всем имеющимся в 
ней полям
