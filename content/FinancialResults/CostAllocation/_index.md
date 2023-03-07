---
title: "Распределение затрат"
draft: false
weight: 8
---

Документы **"Распределение затрат"** предназначены для распределения затрат по аналитикам отгруженной продукции. Распределение используется для формирования финансового результата.

Документы **"Распределение затрат"** расположены в разделе **"Деньги"** в подсистеме **"Закрытие месяца"**:

[![1][1]][1]

В документе можно указать [сценарий](https://konstanta-it.github.io/erp4food/FinancialResult/CostAllocationScenario), остальные поля документа будут заполнены по нему автоматически. Кнопка **"Заполнить и распределить"** позволяет выполнить заполнение таблиц **"Затраты"**, **"База"** и распределить затраты в соответсвии с выбранным сценарием одним действием.

Если сценария нет, то заполняются поля:

- [Организация](https://konstanta-it.github.io/erp4food/CommonInformation/Organization)
- [Направление деятельности](https://konstanta-it.github.io/erp4food/FinancialResult/DirectionOfActivity)

На вкладке **"Затраты"** заполняются отборы:

- По дате: либо устанавливается признак **"На конец месяца"**, тогда затраты будут заполняться на конец месяца, либо заполняется поле **"На"** - элемент справочника **Варианты начала периода**, который отвечает за дату на которую расчитываются затраты

[![2][2]][2]

- [Подразделение](https://konstanta-it.github.io/erp4food/CommonInformation/Department) - отвечает за то по каким подразделениям будут выбираться затраты
- [Статья затрат](https://konstanta-it.github.io/erp4food/FinancialResult/ItemsOfExpenditure) - отвечает за отбор затрат по указанным статьям
- Аналитика затрат - отвечает за отбор затрат по указанным аналитикам
- Отбор - позволяет установить дополнительные отборы
- Сортировка - позволяет задать порядок затрат

[![3][3]][3]

Далее по кнопке **"Заполнить"** табличная часть заполняется затратами согласно установленным отборам, заполняются поля:

- [Подразделение](https://konstanta-it.github.io/erp4food/CommonInformation/Department)
- [Статья затрат](https://konstanta-it.github.io/erp4food/FinancialResult/ItemsOfExpenditure)
- Аналитика затрат
- Сумма

[![4][4]][4]

На вкладке **"База"** заполняются отборы:

- По дате: либо устанавливается признак **Месяц документа**, тогда база определяется за весь месяц в который создано распределение затрат, либо устанавливается период расчета базы

[![5][5]][5]

- Признак **"База на каждую строку затрат"** - устанавливается для того, чтобы для каждой строки затрат определялась своя база
- В таблице устанавливаются отборы по которым определяется база (например, если распределяются затраты на доставку нам сторонней транспортной компанией, то базу нужно расчитывать по Перевозчику):

    - Торговый представитель - менеджер [точки доставки](https://konstanta-it.github.io/erp4food/CommonInformation/DeliveryPoint)
    - Менеджер направления - менеджер группы партнеров для планирования
    - Менеджер клиента - менеджер [контрагента](https://konstanta-it.github.io/erp4food/CommonInformation/Contractor)
    - [Товарная категория](https://konstanta-it.github.io/erp4food/CommonInformation/РroductCategory)
    - Маркетинговое мероприятие
    - [Перевозчик](https://konstanta-it.github.io/erp4food/CommonInformation/Contractor)
    - Транспортное средство
    - Водитель
    - [Задание на доставку](https://konstanta-it.github.io/erp4food/CRM/CustomerService/FormationOfShipments/PlanningOfShipments/DistributionOfShipmentsByCar)
    - [Холдинг](https://konstanta-it.github.io/erp4food/CommonInformation/Holding)
    - [Контрагент](https://konstanta-it.github.io/erp4food/CommonInformation/Contractor)
    - [Заказ клиента](https://konstanta-it.github.io/erp4food/CRM/CustomerService/FormationOfOrders/CustomerOrder)
    - [Подразделение](https://konstanta-it.github.io/erp4food/CommonInformation/Department)
    - Отбор - позволяет установить дополнительные отборы
    - Сортировка - позволяет задать порядок базы

[![6][6]][6]

По кнопке **"Заполнить"** табличная часть вкладки заполняется отгрузками по установленным отборам согласно аналитикам затрат, заполняются поля:

- [Номенклатура](https://konstanta-it.github.io/erp4food/CommonInformation/Nomenclature)
- [Контрагент](https://konstanta-it.github.io/erp4food/CommonInformation/Contractor)
- [Заказ клиента](https://konstanta-it.github.io/erp4food/CRM/CustomerService/FormationOfOrders/CustomerOrder)
- [Документ продаж](https://konstanta-it.github.io/erp4food/CRM/CustomerService/FormationOfShipments/ProductsShipment)
- [Подразделение](https://konstanta-it.github.io/erp4food/CommonInformation/Department)
- Количество
- Сумма
- Вес
- Себестоимость
- Валовая прибыль

[![7][7]][7]

На вкладке **"Расходы"** заполняются:

- Показатель:

    - Количество - затраты будут распределяться пропорционально количеству отгружаемого товара
    - Сумма - затраты будут распределяться пропорционально сумме за отгружаемый товар
    - Вес - затраты будут распределяться пропорционально весам отгружаемого товара
    - Себестоимость - затраты будут распределяться пропорционально себестоимости отгружаемого товара
    - Валовая прибыль - затраты будут распределяться пропорционально валовой прибыли от отгружаемого товара

- Пояснение - произвольный комментарий

По кнопке **"Распределить"** на вкладке табличная часть заполняется распределенными по базе затратами, заполняются поля:

- [Подразделение](https://konstanta-it.github.io/erp4food/CommonInformation/Department)
- [Контрагент](https://konstanta-it.github.io/erp4food/CommonInformation/Contractor)
- [Заказ клиента](https://konstanta-it.github.io/erp4food/CRM/CustomerService/FormationOfOrders/CustomerOrder)
- [Номенклатура](https://konstanta-it.github.io/erp4food/CommonInformation/Nomenclature)
- [Статья затрат](https://konstanta-it.github.io/erp4food/FinancialResult/ItemsOfExpenditure)
- Аналитика затрат
- Показатель
- Сумма

[![8][8]][8]

[1]: 1.png
[2]: 2.png
[3]: 3.png
[4]: 4.png
[5]: 5.png
[6]: 6.png
[7]: 7.png
[8]: 8.png
