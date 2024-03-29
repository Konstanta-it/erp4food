# Мониторинг отгрузки

Для отслеживания и изменения статусов отгрузок товара со склада используется обработка **"Мониторинг отгрузки"**, которая расположена в разделе **"Склад и доставка"** в подсистеме **"Складская логистика"**.

[![1][1]][1]

После открытия обработки заполняются или изменяются следующие поля в верхней части рабочей области в разделе **"Отборы"**:

- Период
- Склад

На форме слева выводятся созданные ранее в системе менеджером **"Планы отгрузки"** сгруппированные по транспортным средствам, если для них сформировано **"Задание на доставку"**. Если по **"Плану отгрузки"** доставка не требуется, то данные документы попадут в группировку **"Не требуется"**. 

[![1(1)][1(1)]][1(1)]

Для того, чтобы перевести **"План отгрузки"** в статус **"Набирается"** необходимо распечатать **"План отгрузки"** и передать его на склад. В системе документ переходит в статус **"Набирается"** после нажатия кнопки **"Печать"**. 

[![2][2]][2]

<h2> Создание документа "Распоряжение на перемещение" с типом Отбор </h2>

На форме обработки так же предусмотрена возможность создания **"Распоряжения на перемещение"** по типу **отбор**, чтобы можно было переместить товар в ячейку отгрузки. Для перехода к форме обработки **"Формирование распоряжений на перемещение по Отбору"** в обработке **"Мониторинг отгрузки"** достаточно нажать на кнопку **"Сформировать распоряжения"**.

[![3][3]][3]

После открытия формы **"Формирование распоряжений на перемещение по Отбору"** необходимо заполнить поля **"Склад"** и решить - нужно ли разделять распоряжения на перемещение по ячейкам (то есть если товар размещен в разных ячейках, то для каждой такой ячейки сформируется свое распоряжение на перемещение), а затем нажать на кнопку **"Заполнить"**. 

После нажатия на кнопку в таблице нижней части формы появится список перемещаемой номенклатуры и информация о том между какими ячейками происходит перемещение.

[![4][4]][4]

Далее надо нажать на кнопку **"Создать документы"**, сформируется распоряжение на перемещение с типом **отбор** у которого будет заполнена вкладка **"План"** и будет установлен статус **"К выполнению"**.

[![5][5]][5]

Перемещение будет выполнено после того как будет заполнена вкладка **"Факт"** и документ будет переведен в статус **"Выполнено"**.

Вернувшись на форму обработки **"Мониторинг отгрузки"** в нижней части можно увидеть какие **"Распоряжения на перемещение"** были созданы.

[![6][6]][6]

<h2>  Отбор под отгрузку </h2>

**"Отбор под перемещение"** используется только на складах с адресной системой хранения при перемещении продукции в ячейку отгрузки под план отгрузки.

После открытия формы обработки **"Меню учетных точек"** заполняем поля:

- Дата
- Смена
- Учетная точка

На форме обработки появятся кнопки выбранной учетной точки, выбираем кнопку **"Отбор под перемещение"**.

[![7][7]][7]

На открывшейся форме надо нажать кнопку **"Обновить"**, будут выведены документы **"План отгрузки"** . В списке при помощи кнопок **"Вверх"** и **"Вниз"** переходим к плану отгрузки для которого будем делать перемещение в ячейку отгрузки, нажимаем кнопку **"Выбрать"**.

[![8][8]][8]

Далее то откроется следующая форма, на ней  надо нажать кнопку **"Обновить"**,  после чего будут выведены документы **"Распоряжения на перемещения"** с типом **"Отбор"**. В списке при помощи кнопок **"Вверх"** и **"Вниз"** переходим к распоряжению на перемещение, нажимаем кнопку **"Выбрать"**.

[![9][9]][9]

Сканируем ячейку из которой будем перемещать товар.

[![10][10]][10]

Далее сканируем штрихкод короба перемещаемой продукции, номенклатура появится на форме.

[![11][11]][11]

Для завершения работы по перемещению нажимаем кнопку **"Завершить"**.

[![12][12]][12]

В  **"Распоряжении на перемещение"** заполнится вкладка **"Факт"** и документ будет переведен в статус **"Выполнено"**.

[![13][13]][13]

[![14][14]][14]

В **"Мониторинге отгрузке"** будет отображено отобранное количество.

После чего переводим документ **"План отгрузки"** в статус **"Собрано"** 

[![15][15]][15]

<h2>  Формирование распоряжения на отгрузку </h2>

Для **"Заказов на перемещение"** не требующих доставки в АРМе **"Мониторинг отгрузки"** предусмотрена кнопка **"Сформировать отгрузку по наборке"**. По нажатию этой кнопки автоматически сформируется **"Распоряжение на отгрузку"** на основании фактических данных из **"Распоряжения на перемещение"** по типу Отбор.

Для **"Заказов на перемещение"**, по которым оформлены **"Задания на доставку"** осуществляется Отгрузка на ТСД.

После открытия формы обработки **"Меню учетных точек"** заполняем поля:

- Дата
- Смена
- Учетная точка

На форме обработки появятся кнопки выбранной учетной точки, выбираем кнопку **"Отгрузка"**.

[![16][16]][16]

На открывшейся форме по нажатию кнопки **"Обновить"**, будут выведены документы **"План отгрузки"**. В списке при помощи кнопок **"Вверх"** и **"Вниз"** переходим к плану отгрузки по которому будем делать отгрузку, нажимаем кнопку **"Выбрать"**.

[![17][17]][17]

Далее сканируем штрихкод короба отгружаемой со склада продукции, номенклатура появится на форме. (Вводим в поле "Штрихкод" SSCC код наших коробов по очереди).

[![18][18]][18]

Для завершения работы по отгрузке нажимаем кнопку **"Завершить"**.

[![19][19]][19]

В результате будет заполнен документ **"Распоряжение на отгрузку"**.

[![20][20]][20]

В **"Мониторинге отгрузке"** будет отображено фактическое количество.

После чего переводим документ **"План отгрузки"** в статус **"Погружено"** 

[![21][21]][21]

[1]: ShipmentMonitoring.assets/1.png
[1(1)]: ShipmentMonitoring.assets/1(1).png
[2]: ShipmentMonitoring.assets/2.png
[3]: ShipmentMonitoring.assets/3.png
[4]: ShipmentMonitoring.assets/4.png
[5]: ShipmentMonitoring.assets/5.png
[6]: ShipmentMonitoring.assets/6.png
[7]: ShipmentMonitoring.assets/7.png
[8]: ShipmentMonitoring.assets/8.png
[9]: ShipmentMonitoring.assets/9.png
[10]: ShipmentMonitoring.assets/10.png
[11]: ShipmentMonitoring.assets/11.png
[12]: ShipmentMonitoring.assets/12.png
[13]: ShipmentMonitoring.assets/13.png
[14]: ShipmentMonitoring.assets/14.png
[15]: ShipmentMonitoring.assets/15.png
[16]: ShipmentMonitoring.assets/16.png
[17]: ShipmentMonitoring.assets/17.png
[18]: ShipmentMonitoring.assets/18.png
[19]: ShipmentMonitoring.assets/19.png
[20]: ShipmentMonitoring.assets/20.png
[21]: ShipmentMonitoring.assets/21.png
