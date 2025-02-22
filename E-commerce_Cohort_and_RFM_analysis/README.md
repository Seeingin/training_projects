**Анализ данных о продажах, проведение когортного анализа, построение RFM-сегментации**
=====================

**Цели:**
<li>
выгрузить и изучить имеющиесяя данные
<li>
исследовать данные на наличие аномалий
<li>
принять и обосновать решения о трактовке спорных моментов в данных
<li>
определить, сколько пользователей совершили покупку только один раз
<li>
определить, сколько заказов в месяц в среднем не доставляется по разным причинам 
<li>
по каждому товару определить, в какой день недели товар чаще всего покупается
<li>
определить, сколько у каждого из пользователей в среднем покупок в неделю (по месяцам)
<li>
провести когортный анализ пользователей
<li>
построить RFM-сегментацию пользователей
<li>
визуализировать полученные результаты
<li>
сформулировать выводы

**Описание данных:**

1. *olist_customers_datase.csv* — таблица с уникальными идентификаторами пользователей
customer_id — позаказный идентификатор пользователя

customer_unique_id —  уникальный идентификатор пользователя  (аналог номера паспорта)

customer_zip_code_prefix —  почтовый индекс пользователя

customer_city —  город доставки пользователя

customer_state —  штат доставки пользователя

2. *olist_orders_dataset.csv* —  таблица заказов
order_id —  уникальный идентификатор заказа (номер чека)

customer_id —  позаказный идентификатор пользователя

order_status —  статус заказа

order_purchase_timestamp —  время создания заказа

order_approved_at —  время подтверждения оплаты заказа

order_delivered_carrier_date —  время передачи заказа в логистическую службу

order_delivered_customer_date —  время доставки заказа

order_estimated_delivery_date —  обещанная дата доставки

3. *olist_order_items_dataset.csv* —  товарные позиции, входящие в заказы
order_id —  уникальный идентификатор заказа (номер чека)

order_item_id —  идентификатор товара внутри одного заказа

product_id —  ид товара (аналог штрихкода)

seller_id — ид производителя товара

shipping_limit_date —  максимальная дата доставки продавцом для передачи заказа партнеру по логистике

price —  цена за единицу товара

freight_value —  вес товара

*Уникальные статусы заказов в таблице olist_orders_dataset*:

created —  создан

approved —  подтверждён

invoiced —  выставлен счёт

processing —  в процессе сборки заказа

shipped —  отгружен со склада

delivered —  доставлен пользователю

unavailable —  недоступен

canceled —  отменён

**Используемые библиотеки**

`pandas` `numpy` `requests` `datetime` `calendar` `matplotlib` `plotly`

