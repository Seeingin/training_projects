**Финальный проект Karpov.Courses**
=====================

**Кейс 1. A\B тест**

Анализ результатов А\В теста по внедрению новой механика оплаты услуг на сайте, формулирование выводов и рекомендаций.

**Описание данных:**
1. *groups.csv* - файл с информацией о принадлежности пользователя к контрольной или экспериментальной группе (А – контроль, B – целевая группа) 

2. *groups_add.csv* - дополнительный файл с пользователями, который вам прислали спустя 2 дня после передачи данных

3. *active_studs.csv* - файл с информацией о пользователях, которые зашли на платформу в дни проведения эксперимента. 

4. *checks.csv* - файл с информацией об оплатах пользователей в дни проведения эксперимента. 

**Кейс 2. SQL**

Подключение к БД ClickHouse, выгрузка необходимых данных, подсчет следующих метрик с помощью SQL-запроса:
* ARPU 

* ARPAU 

* CR в покупку 

* СR активного пользователя в покупку 

* CR пользователя из активности по математике (subject = ’math’) в покупку курса по математике

**Кейс 3. Python**

* Реализация функции для автоматической подгрузки информации из дополнительного файла groups_add.csv и пересчитывания метрик (ARPU, ARPAU, CR) на основании дополнительных параметров.

* Реализация функции для построения графиков по получаемым метрикам.

**Используемые библиотеки**

`pandas`  `numpy` `seaborn` `matplotlib` `requests` `urlencode` `pandahouse` `scipy`
