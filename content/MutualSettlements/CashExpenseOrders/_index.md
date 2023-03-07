---
title: "Расходные кассовые ордера"
draft: false
weight: 6
---

Для регистрации расходов наличных денежных средств из кассы организации предназначен документ **"Расходный кассовый ордер"**.

Документы **"Расходные кассовые ордера"** расположены в разделе **"Деньги"** - **"Кассы"**.

[![1][1]][1]

В документе заполняются поля:

- Номер - заполняется автоматически при сохранении
- Дата
- Вид операции - влияет на состав реквизитов документов. Возможны 5 видов операций:

    - ***Возврат оплаты клиенту***, в документе заполняются реквизиты:

        - [Организация](https://konstanta-it.github.io/erp4food/CommonInformation/Organization)
        - [Подразделение](https://konstanta-it.github.io/erp4food/CommonInformation/Department)
        - Касса
        - [Контрагент](https://konstanta-it.github.io/erp4food/CommonInformation/Contractor)
        - Сумма документа
        - Валюта
        - Дата платежа

        [![2][2]][2]

        На вкладке **"Расшифровка платежа"** табличная часть заполняется следующими данными:

        - Основание - [соглашение с контрагентом](https://konstanta-it.github.io/erp4food/CRM/CustomerService/Pricing/AgreementsWithContractors)
        - Объект расчета - объект по которому будет зачтена оплата от клиента, это могут быть [соглашение с контрагентом](https://konstanta-it.github.io/erp4food/CRM/CustomerService/Pricing/AgreementsWithContractors) или [реализации товаров](https://konstanta-it.github.io/erp4food/CRM/CustomerService/FormationOfShipments/FormationOfTheAccompanyingDocuments/FormationOfTheImplementationsOfProducts)
        - Сумма
        - [Статья ДДС](https://konstanta-it.github.io/erp4food/MutualSettlements/CashFlowItems)

        [![3][3]][3]

    - ***Прочие расходы***, в документе заполняются поля:

        - [Организация](https://konstanta-it.github.io/erp4food/CommonInformation/Organization)
        - [Подразделение](https://konstanta-it.github.io/erp4food/CommonInformation/Department)
        - Касса
        - Сумма документа
        - Валюта
        - Дата платежа

        [![4][4]][4]

    - ***Выдача подотчетнику***, в документе заполняются поля:

        - [Организация](https://konstanta-it.github.io/erp4food/CommonInformation/Organization)
        - [Подразделение](https://konstanta-it.github.io/erp4food/CommonInformation/Department)
        - Касса
        - Подотчетное лицо
        - Сумма документа
        - Валюта
        - Дата платежа

        [![5][5]][5]

    - ***Списание по результатам инвентаризации***, в документе заполняются поля:

        - [Организация](https://konstanta-it.github.io/erp4food/CommonInformation/Organization)
        - [Подразделение](https://konstanta-it.github.io/erp4food/CommonInformation/Department)
        - Касса
        - [Инвентаризация](https://konstanta-it.github.io/erp4food/MutualSettlements/CashInventory)
        - Сумма документа
        - Валюта
        - Дата платежа

        [![6][6]][6]

    - ***Инкассация в банк***, в документе заполняются поля:

        - [Организация](https://konstanta-it.github.io/erp4food/CommonInformation/Organization)
        - [Подразделение](https://konstanta-it.github.io/erp4food/CommonInformation/Department)
        - Касса
        - Банковский счет
        - Сумма документа
        - Валюта
        - Дата платежа

        [![7][7]][7]

Для **"Расходных кассовых ордеров"** со всеми видами операций заполняется вкладка "Печать"

[![8][8]][8]

и может быть распечатан "Расходный кассовый ордер"

[![9][9]][9]

[1]: 1.png
[2]: 2.png
[3]: 3.png
[4]: 4.png
[5]: 5.png
[6]: 6.png
[7]: 7.png
[8]: 8.png
[9]: 9.png
