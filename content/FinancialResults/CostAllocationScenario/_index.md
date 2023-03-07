---
title: "Сценарии распределения затрат"
draft: false
weight: 5
--- 

Справочник **"Сценарий распределения затрат"** используется для хранения настроек [распределения затрат](https://konstanta-it.github.io/erp4food/FinancialResult/CostAllocation).

Справочник расположен в разделе **"Деньги"** в подсистеме **"Закрытие месяца"**

[![1][1]][1]

Для сценария распределения затрат указываются:

- Наименование - используется для представления объекта в системе
- [Организация](https://konstanta-it.github.io/erp4food/CommonInformation/Organization)
- [Направление деятельности](https://konstanta-it.github.io/erp4food/FinancialResult/DirectionOfActivity)
- Пояснение - произвольный комментарий

На вкладке **"Затраты"** устанавливается либо признак **"Остаток на конец месяца"**, тогда затраты в документе [**"Распределение затрат"**](https://konstanta-it.github.io/erp4food/FinancialResult/CostAllocation) будут заполняться на конец месяца, либо заполняется поле **"Остаток затрат на дату"** - элемент справочника **Варианты начала периода**, который отвечает за дату на которую расчитываются затраты

В табличной части вкладки **"Затраты"** могут быть заполнены отборы:

- [Подразделение](https://konstanta-it.github.io/erp4food/CommonInformation/Department) - отвечает за то по каким подразделениям будут выбираться затраты
- [Статья затрат](https://konstanta-it.github.io/erp4food/FinancialResult/ItemsOfExpenditure) - отвечает за отбор затрат по указанным статьям
- Аналитика затрат - отвечает за отбор затрат по указанным аналитикам
- Отбор - позволяет установить дополнительные отборы
- Сортировка - позволяет задать порядок затрат

[![2][2]][2]

На вкладке **"База"** заполняются:

- Показатель:

    - Количество - затраты будут распределяться пропорционально количеству отгружаемого товара
    - Сумма - затраты будут распределяться пропорционально сумме за отгружаемый товар
    - Вес - затраты будут распределяться пропорционально весам отгружаемого товара
    - Себестоимость - затраты будут распределяться пропорционально себестоимости отгружаемого товара
    - Валовая прибыль - затраты будут распределяться пропорционально валовой прибыли от отгружаемого товара

- Признак **"База на каждую строку затрат"** - устанавливается для того, чтобы для каждой строки затрат определялась своя база

- Фиксированная или Рассчитываемая

    Если база **Фиксированная**, то таблица вручную заполняется данными:

    - [Подразделение](https://konstanta-it.github.io/erp4food/CommonInformation/Department)
    - [Контрагент](https://konstanta-it.github.io/erp4food/CommonInformation/Contractor)
    - [Заказ клиента](https://konstanta-it.github.io/erp4food/CRM/CustomerService/FormationOfOrders/CustomerOrder)
    - Аналитика
    - Количество
    - Сумма
    - Вес
    
    Если база **Рассчитываемая**, то либо устанавливается признак **База распределения на месяц документа**, тогда база определяется за весь месяц в который создано [распределение затрат](https://konstanta-it.github.io/erp4food/FinancialResult/CostAllocation), либо устанавливается период расчета базы

    В табличной части устанавливаются отборы по которым определяется база (например, если распределяются затраты на доставку нам сторонней транспортной компанией, то базу нужно расчитывать по Перевозчику):

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

[![3][3]][3]

[1]: 1.png
[2]: 2.png
[3]: 3.png
