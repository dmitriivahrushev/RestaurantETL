**Gastro Hub**
--
![Gastro Hub](png/hub.png)
**Описание проекта**
--
**В файле дампа содержатся данные о сети ресторанов Gastro Hub.**
--
~~~bash
dump_gastrohub.sql
~~~
raw_data.sales — необработанные данные о продажах
--
report_date Дата `date`  
type Тип заведения `character varying`  
cafe_name	Название заведения `character varying`  
avg_check	Средний чек за день `numeric(6, 2)`  
manager	Ф. И. О менеджера заведения `character varying`  
manager_phone	Телефон менеджера заведения `character varying`   

**raw_data.menu — необработанные данные о меню заведений**  
--
cafe_name	Название заведения  `character varying`  
menu	Меню  `jsonb`

**ERD-диаграмма нормализованных таблиц**
--
![ERD](png/erd.png)
--
Таблица `cafe.restaurants` содержит информацию о ресторанах.  
Поля: restaurant_uuid, название заведения, тип заведения и меню.

Таблица `cafe.managers` содержит информацию о менеджерах.  
Поля: manager_uuid, имя менеджера и его телефон.

Таблица `cafe.restaurant_manager_work_dates` таблица хранит дату начала работы в ресторане и дату окончания работы в ресторане.
Поля: restaurant_uuid, manager_uuid, работа менеджера в ресторане от даты начала до даты окончания — единый период, без перерывов.

Таблица `cafe.sales` хранит даты и средний чек заведения.

- DDL.sql - запросы на создание схемы `cafe` и объектов в ней в нужном порядке.
- INSERT.sql - запросы на заполнение таблиц данными.
- task_1.sql - task_7.sql - решения заданий в порядке их выполнения.




