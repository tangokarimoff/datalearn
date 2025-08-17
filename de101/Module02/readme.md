#   Задания Модуля 2
---
## 2.3. Подключение к Базам Данных и SQL
1. _Устанавливаем PostgreSQL 17 и клиент DBeaver для подключения к БД._
2. *Создаем три таблицы и загружаем данные c помощью запросов в DBeaver*
     
**Cкрипты загрузки данных:**
  + [script_table_orders.sql](https://github.com/tangokarimoff/datalearn/blob/a4cb128b366045d952945a28b1c95f94241d3f13/de101/Module02/script_table_orders), 
  + [script_table_people.sql](https://github.com/tangokarimoff/datalearn/blob/a4cb128b366045d952945a28b1c95f94241d3f13/de101/Module02/script_table_people), 
  + [script_table_returns.sql](https://github.com/tangokarimoff/datalearn/blob/a4cb128b366045d952945a28b1c95f94241d3f13/de101/Module02/script_table_returns)
---
## 2.4. Модель данных.
Задача создать модель данных для файла с данными [superstore.xls](https://github.com/tangokarimoff/datalearn/blob/81f351348549390229ce3b9c37c159f4cd222584/de101/Module02/Superstore.xls).

_Для архитектуры БД выбрана схема "Звезда" по Инману. Создаем Dimensions таблицы, далее Sales_fact._

- **Концептуальная модель.**

_Определяем основные элементы. Можно сказать,составляем скорее диагрмму основных бизнес процессов   
(Что происходит между элементами?). Намечаем границы будущих таблиц._

![concept data model](https://github.com/tangokarimoff/datalearn/blob/3ac01fcb34dc3adc4ccf122f8b56e537f8a5978a/de101/Module02/img/ConceptModel.png)

- **Физическая модель.**

_Добавление синтаксиса. Можно сказать,что данный этап непосредственно является DDL._

![physical data model](https://github.com/tangokarimoff/datalearn/blob/3ac01fcb34dc3adc4ccf122f8b56e537f8a5978a/de101/Module02/img/PhysModel.png)

- **Generate SQL.**

_Генерируем SQL-запросы --> DDL. Выполняем в SQL клиенте._

- **Делаем ```insert into table```.**

_Заполняем Dimensions и Sales_fact._

[Create script_datamodeling_DDL.sql](https://github.com/tangokarimoff/datalearn/blob/3ac01fcb34dc3adc4ccf122f8b56e537f8a5978a/de101/Module02/script_datamodeling_DDL)- файл со скриптом.
