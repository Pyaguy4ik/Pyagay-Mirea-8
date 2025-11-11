# Практическое задание № 8

# Работа с MongoDB: подключение, создание коллекции, CRUD-операции

Студент группы *ЭФМО-02-25 Пягай Даниил Игоревич*

# Описание

**Цели:**

    • Понять базовые принципы документной БД MongoDB (документ, коллекция, BSON, _id:ObjectID).
    • Научиться подключаться к MongoDB из Go с использованием официального драйвера.
    • Создать коллекцию, индексы и реализовать CRUD для одной сущности (например, notes).
    • Отработать фильтрацию, пагинацию, обновления (в т.ч. частичные), удаление и обработку ошибок.


## Инициализация проекта

```bash
mkdir pz7-redis
cd pz7-redis
go mod init example.com/pz7-redis
go get github.com/redis/go-redis/v9
```

## Создаём структуру файлов

![structure](img/structure.png)

# Запускаем сервер и проверяем

## Запрос /Health
![create](img/health.png)

## Создаём 2 заметки
![create](img/create_note.png)
![create](img/create_note_2.png)

## Получаем список
![Set](img/all_notes.png)

## Получаем по id
![Get](img/search_id.png)

## Частичное обновление
![ttl](img/update_context.png)

## Удаление
![ttl](img/delete.png)

## Проверка по id после удаления
![ttl](img/after_delete.png)
