**Gastro Hub**
--
![Gastro Hub](png/image.jpeg)
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

- DDL.sql - запросы на создание схемы `cafe` и объектов в ней в нужном порядке.
- INSERT.sql - запросы на заполнение таблиц данными.
- task_1.sql - task_7.sql - решения заданий в порядке их выполнения.




