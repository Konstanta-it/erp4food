---
title: "Приемка заказов"
draft: false
weight: 2
---

Документ **"Заказ клиента"** отражает потребность клиента на поставку ему товаров. Они расположены в разделе **"Заказы"**.

![1](1.png)

Для пользователей, которые занимаются созданием заказов клиентов в системе создан поставляемый профиль доступа *"Создание заказов клиента"*.

![2](2.png)

!!! attention ""
    В данном профиле нет роли **"Разрешено изменять цены в документах"**, которая позволяет вручную изменять цены в заказе на отличные от установленных по соглашению.

!!! attention ""
    Чтобы предоставить пользователю, создающему заказы возможность изменения цен нужно создать профиль, включающий роль **"Разрешено изменять цены в документах"** и добавить его для пользователя.

При создании документа указываются:

**Вкладка "Основное"**

- Номер - заполняется автоматически
- Дата
- [Организация](https://konstanta-it.github.io/erp4food/CommonInformation/Organization)
- [Подразделение](https://konstanta-it.github.io/erp4food/CommonInformation/Department)
- [Холдинг](https://konstanta-it.github.io/erp4food/CommonInformation/Holding)
- [Контрагент](https://konstanta-it.github.io/erp4food/CommonInformation/Contractor)
- [Соглашение об условиях продаж](https://konstanta-it.github.io/erp4food/CRM/CustomerService/Pricing/AgreementsWithContractors)
- [Бизнес-регион](https://konstanta-it.github.io/erp4food/CommonInformation/BusinessRegion) - указывается из соглашения
- [Точка доставки](https://konstanta-it.github.io/erp4food/CommonInformation/DeliveryPoint)
- Тип доставки - заполняется из точки доставки, можно заполнить вручную (Самовывоз, Доставка сторонней транспортной компанией, Доставка нашей транспортной компанией)
- Информация о цене - заполняется из соглашения
- Дата отгрузки
- Дата доставки

**Вкладка "Товары"**

Список заказываемой номенклатуры. Заполняется номенклатура, её характеристика, количество, упаковка, цены рассчитываются автоматически на основании соглашения об условиях продаж, из точки доставки автоматически устанавливается склад отгрузки.

В нижней части формы документа заполняется комментарий, рассчитываются: скидка, процент скидки, сумма НДС, итоговая сумма заказа.

Создадим заказ клиента, заполнив его данными:

- Дата - 29.05.2020
- Организация - Молочный мир
- Контрагент - ООО "АШАН"
- Соглашение об условиях продаж - АШАН. Соглашение об условии продаж
- Точка доставки - АШАН, Родионова, 187
- Тип доставки - Доставка нашей транспортной компанией
- Дата отгрузки - 29.05.2020
- Дата доставки - 29.05.2020

![3](3.png)

Далее переходим к табличной части товары и заполняем её:

- Сыр Адыгейский, количество - 10, упак - 1 кг
- Сыр Костромской, количество - 10, упак - 1 кг
- Сыр Пошехонский, количество - 10, упак - 1 кг

Остальные поля будут заполнены автоматически.

![4](4.png)

Сохраняем документ, для этого нажимаем кнопку **"Провести и закрыть"**.

![5](5.png)

Для документа **"Заказ клиента"** используются печатные формы: *"Заказ клиента"*, *"Счет на оплату (выводить скидки)"*, *"Счет на оплату (не выводить скидки)"*.

![6](6.png)

Заказы клиентов могут быть загружены из exel - из файла или из бланка.

![7](7.png)

Регламентированным вводом заказов является их загрузка из бланка. Для проектов создаются стандартные бланки, которые выгружаются и отправляются клиентам. Клиенты указывают количество заказываемых товаров в бланке и возвращают обратно. Полученный от клиента бланк заказа загружается в систему.

Для выгрузки бланков создаются **"Настройки выгрузки заказов"**, которые расположены в разделе **Заказы** в подсистеме **"Сервис"** - **"Настройки исполнения заказов"**

![8](8.png)

![9](9.png)

Для **"Настроек выгрузки заказов"** заполняются:

- Наименование
- Признак отправки на почту

В табличной части заполняются:

- [Точки доставки](https://konstanta-it.github.io/erp4food/CommonInformation/DeliveryPoint)
- Каталоги в которые выгружаются бланки
- Почта - заполняется из карточки [контрагента](https://konstanta-it.github.io/erp4food/CommonInformation/Contractor)

![10](10.png)

Бланки для заказов создаются в АРМе *"Создание бланков заказов"*, который расположен в разделе **"Заказы"**.

![11](11.png)

На вкладке **"Настройки"** заполняются дата (дата доставки), организация, подразделение, признак - защищать бланки, настройки каталога товаров.

Признак **защищать бланки** позволяет защитить от редактирования все колонки таблицы товаров выгружаемого бланка кроме количества.

Настройки каталога товаров включают в себя условия на товары, которые будут указаны в бланке:

- Только с ценой (в бланке будут указаны только те товары на которые установлена цена на дату отгрузки по виду цены из соглашения с контрагентом, для заказов на перемещение действует цена указанная для перемещений в настройках исполнения заказов клиентов)
- Доступные по сезонам (в бланке будут указаны товары для которых не установлен сезон или для которых дата отгрузки попадает в сезон)
- Только из спецификации (в бланке будут указаны товары, которые указаны в регистре "Спецификации соглашений с клиентами" для соглашения с контрагентом)
- Доступные для продажи (в бланке окажется номенклатура для которой дата отгрузки попадает в диапазон между датами ввода в продажу и вывода из продажи)

![12](12.png)

На вкладке **"Заказы клиентов"** по кнопке **"Подобрать настройки"** выбираются настройки выгрузки заказов. По настройкам заполняются точка доставки, соглашение с контрагентом и каталог куда будет выгружен бланк. Так же эти данные могут быть заполнены вручную.

![13](13.png)

Нажимаем кнопку **"Сформировать бланки"**, в выбранном каталоге появится бланк с названием в котором указаны соглашение и дата отгрузки.

![14](14.png)

На вкладке **"Заказы на перемещение"** формируются бланки для заказов на перемещение товаров.

В таблице товаров указывается количество заказываемых товаров.

![15](15.png)

При загрузке бланка указывается каталог из которого будет загружен бланк и каталог в который этот бланк будет перемещен после загрузки.

![16](16.png)

При загрузке создается заказ клиента.

![17](17.png)

![18](18.png)

Характеристика номенклатуры заполняется автоматически только для контрагентов для которых созданы характеристики.

При загрузке бланка с той же датой отгрузки, точкой доставки и соглашением повторно данные в старом заказе будут изменены на загружаемые.

Заказы клиентов могут быть загружены регламентным заданием **"Загрузка заказов из бланков"**

![19](19.png)

Для этого нужно заполнить **"Настройки загрузки заказов"**, которые расположены в разделе **Заказы** в подсистеме **"Сервис"** - **"Настройки исполнения заказов"**

![8](8.png)

![20](20.png)

Для **"Настроек загрузки заказов"** заполняются:

- Наименование
- Признак автоматической загрузки
- Признак создания одного заказа на дату
- Путь к папке загрузки
- Путь к папке обработанных бланков

![21](21.png)

**"Настройки загрузки заказов"** указываются для контрагента:

![22](22.png)

При запуске регламентного задания **"Загрузка заказов из бланков"** в систему загружаются заказы клиентов согласно настройкам.

Для заказов клиентов можно включить **"Контроль остатков заказов"** в разделе **Заказы** в подсистеме **"Сервис"** - **"Настройки исполнения заказов"**

![8](8.png)

![23](23.png)

Данная настройка не позволяет после оформления по заказу [плана отгрузки](https://konstanta-it.github.io/erp4food/CRM/CustomerService/FormationOfShipments/PlanningOfShipments/CreationOfPlansForShipment) сделать количество товаров в заказе клиента меньше чем в плане:

![24](24.png)

При этом количество в плане отгрузки нельзя сделать больше чем в заказе:

![25](25.png)
