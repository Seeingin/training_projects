**Построение воронки продаж и расчет конверсии клиентов квеста**
=====================

**Цели:**
<li>
исследовать данные
<li>
выгрузить данные из БД SQL-запросом
<li>
рассчитать % конверсии на каждом этапе воронки
<li>
визуализировать полученные данные
<li>
сформулировать выводы и точки роста продукта

**Описание данных:**

База данных содержит информацию о продукте Тинькофф.Квест:

Partner - Витрина содержит информацию о наших бизнес партнерах;
  
Location - Витрина содержит информацию о тех локациях, на которых проходят квесты нашей франшизы;
  
Legend - Витрина содержит информацию о легендах (сценариях/сюжетах) конкретных квестов;
  
Quest - Витрина содержит информацию о квестах, в которые могут играть наши клиенты;
  
Employee - Витрина содержит информацию о сотрудниках, которые проводят игры и помогают командам;
  
Game - Витрина с расписанием запланированных и состоявшихся игр;
  
Client - Витрина содержит информацию о клиентах, посетивших наш сайт;
  
Account - Витрина содержит информацию об аккаунтах клиентов;
  
Application - Витрина содержит информацию о заявках клиентов на иргы

**Используемые библиотеки**

`pandas`  `numpy` `plotly`