### Задание 1. - Создание базы данных c 3 таблицами в mySqlWorkbench

Научиться пользоваться инстументом визуальной работы с БД - mySQLWorkbench  
Учебное видео [Создание базы данных MySQL Workbench](https://www.youtube.com/watch?v=ChLjnsKLoZE)  

1. Найдите в строке поиска `mySQLWorkbench` и запустите программу  
2. Добавьте новую модель `File \ New Model` и переименуйте ее с `myDB` на `ProductDB-TG231B`
3. Добавьте новую диаграмму через `Add diagram`
4. Добавьте новую таблицу (нажав на иконку с изображением таблицы)
```
Название:
user
Поля (Columns):
id INT PK NN AI
name VARCHAR(45)
surname VARCHAR(45)
```
5. Добавьте еще одну таблицу (2-ю)
```
Название:
product
Поля (Columns):
id INT PK NN AI
name VARCHAR(45)
description LONGTEXT
```
6. Добавьте еще одну таблицу (3-ю)
```
Название:
invoice
Поля (Columns):
id INT PK NN AI
user_id INT NN
product_id INT NN
sum FLOAT
```
<hr>

### Задание 2. - Связь между таблицами

Последняя таблица - таблица связи между двумя другими таблицами,   
поэтому для нее надо добавить внешние ключи
```
Foreign keys
user_key user_id CASCADE, CASCADE
product_key product_id CASCADE, CASCADE
```

2. Запустите сервер СУБД `mySQL` через программу `XAMPP Control Panel` (найдите в строке поиска) - нажмите кнопку Start, чтобы надпись mySQL загорелась зеленым
