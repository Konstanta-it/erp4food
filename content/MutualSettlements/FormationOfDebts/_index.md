---
title: "Формирование задолженностей"
draft: false
weight: 3
---

После того как [график оплаты](https://konstanta-it.github.io/erp4food/MutualSettlements/PaymentSchedule) был создан, чтобы он работал нужно его указать в [соглашении с контрагентом](https://konstanta-it.github.io/erp4food/CRM/CustomerService/Pricing/AgreementsWithContractors).

В соглашении с контрагентом на вкладке **"Взаиморасчеты"** заполняются:

- Признак использования взаиморасчетов для расчета задолженности (в проверках заказов клиентов)
- Валюта взаиморасчетов
- Порядок расчетов:

    - По накладным
    - По соглашениям

- [График оплаты](https://konstanta-it.github.io/erp4food/MutualSettlements/PaymentSchedule)

[![1][1]][1]

В [заказе клиента](https://konstanta-it.github.io/erp4food/CRM/CustomerService/FormationOfOrders/CustomerOrder) из соглашения заполняются порядок расчетов, форма оплаты, график оплаты и валюта.

[![2][2]][2]

В [реализации товаров](https://konstanta-it.github.io/erp4food/CRM/CustomerService/FormationOfShipments/FormationOfTheAccompanyingDocuments/FormationOfTheImplementationsOfProducts) из соглашения заполняются порядок расчетов, форма оплаты, график оплаты и валюта. Табличная часть при проведении документа или по нажатию кнопки **"Заполнить по графику"** заполняется информацией о том какими датами и какими суммами ожидаются оплаты от клиента.

Задолженность будет отнесена на соглашение с клиентом или на реализацию в зависимости от выбранного порядка расчета.

[![3][3]][3]

Оформление [корректировки реализации товаров](https://konstanta-it.github.io/erp4food/CRM/CustomerService/FormationOfShipments/FormationOfTheAccompanyingDocuments/AdjustingProductImplementations/AdjustingProductImplementations) меняет сумму задолженности клиента. Задолженность может как увеличиться, так и уменьшиться:

[![4][4]][4]

[Возврат товаров от клиента](https://konstanta-it.github.io/erp4food/CRM/CustomerService/FormationOfAFeedback/ReturnOfProductsFromTheCustomer) уменьшает сумму задолженности клиента:

[![5][5]][5]

[1]: 1.png
[2]: 2.png
[3]: 3.png
[4]: 4.png
[5]: 5.png
