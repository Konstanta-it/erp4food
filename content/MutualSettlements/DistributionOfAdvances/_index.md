---
title: "Распределение авансов"
draft: false
weight: 11
---


Для контрагентов у которых в [соглашении](https://konstanta-it.github.io/erp4food/CRM/CustomerService/Pricing/AgreementsWithContractors) указан порядок расчетов по накладным могут быть оформлены авансы.

[![1][1]][1]

Для оформления авансов создаются документы:

- [Приходный кассовый ордер](https://konstanta-it.github.io/erp4food/MutualSettlements/IncomingCashOrders) с операцией **Поступление оплаты**
- [Поступление безналичных денежных средств](https://konstanta-it.github.io/erp4food/MutualSettlements/IncomingCashOrders)

На вкладке расшифровка платежа в качестве объекта расчета указывается соглашение с клиентом.

[![2][2]][2]

Для распределения авансов по накладным используется кнопка **"Заполнить по задолженностям"**.

[![3][3]][3]

[1]: 1.png
[2]: 2.png
[3]: 3.png
