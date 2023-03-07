---
title: "Подтверждение заказов"
draft: false
weight: 3
---

Для подтверждения количества отгружаемого товара по заказам используется вкладка **"Подтверждение заказов"** АРМа **"Формирование плана отгрузки"**. АРМ расположен в разделе **"Склад и доставка"** в подсистеме **"Складская логистика"**.

[![1][1]][1]

Для пользователей, которые занимаются подтверждением заказов в системе создан поставляемый профиль доступа *"Подтверждение заказов"*.

[![2][2]][2]

Подтверждение заказов происходит по **"Настройкам формирования планов отгрузки"**, которые заполняются в разделе **"Заказы"** в подсистеме **"Сервис"** - **"Настройки исполнения заказов"**.

[![3][3]][3]

[![4][4]][4]

В **"Настройках формирования планов отгрузки"** заполняются:

- Наименование
- Дата отгрузки - элемент справочника **"Варианты начала периода"**, заполняется для определения по дате отгрузки заказов с которыми работаем
- Причина расхождения - причина из-за которой заказы были скорректированы
- Округлять по кратности - при установке признака во время редактирования заказов количество будет округляться к наибольшему ближайшему кратному, кратность устанавливается в регистре "Кратность номенклатуры" или в самой номенклатуре
- Использовать для автоматического подтверждения - при установке признака для заказов удовлетворяющим настройкам регламентным заданием "Автоматическое подтверждение заказов" будут подтверждаться заказы
- Склады отгрузки - перечень складов с которыми работаем
- Этап заказа клиента для чтения - в АРМе будет отображаться количество в заказах клиента из установленного этапа
- Этап заказа клиента для записи - после корректировки результат будет сохранен для данного этапа
- Состояние "Подтверждено" Заказа клиента - состояние которое будет установлено после корректировки для заказов клиентов
- Этап заказа на перемещение для чтения - в АРМе будет отображаться количество в заказах на перемещение из установленного этапа
- Этап заказа на перемещение для записи - после корректировки результат будет сохранен для данного этапа
- Состояние "Подтверждено" Заказа на перемещение - состояние которое будет установлено после корректировки для заказов на перемещение
- Точки доставки - список точек доставки для отбора заказов клиентов с которыми работаем
- Склады получатели - список складов получателей для отбора заказов на перемещение с которыми работаем
- Товарные категории - список товарных категорий для определения номенклатур по которым производится корректировка

Рассмотрим подтверждение заказа клиента на 29.05.2020 для контрагента "ООО "АШАН" с использованием этапов. Заполним **"Настройки формирования планов отгрузки"**, для этого создадим состояние **"Подтверждено"** для заказа клиента:

[![5][5]][5]

В **"Настройках формирования планов отгрузки"** заполняем:

- Наименование - Подтверждение заказов на 29.05.2020
- Дата отгрузки - 29.05.2020
- Причина расхождения - Расхождения при отгрузке
- Округлять по кратности - Истина
- Склады отгрузки - Склад готовой продукции
- Этап заказа клиента для чтения - Исходный
- Этап заказа клиента для записи - Подтвержденный
- Состояние "Подтверждено" Заказа клиента - Заказ клиента подтвержден
- Точки доставки - АШАН, Родионова, 187
- Товарные категории - Мягкие сыры, Молочная продукция, Полутвердые сыры, Твердые сыры

[![6][6]][6]

Обрежем заказ на 29.05.2020 для контрагента "ООО "АШАН" по этапам, переходим к обработке **"Формирование плана отгрузки"** и устанавливаем настройки формирования планов отгрузки в обработке - Подтверждение заказов на 29.05.2020

[![7][7]][7]

Затем нажимаем кнопку **"Обновить"**, в табличной части будет выведена заказанная номенклатура.

[![8][8]][8]

В АРМе **"Формирование планов отгрузки"** на вкладке **"Подтверждение заказов"** есть следующие функции:

1. В контекстном меню, которое вызывается нажатием правой кнопки мыши при выборе заказа в таблице:

    - Обнулить колонку - обнуляется колонка, отвечающая за подтвержденное количество в выбранном заказе
    - Обнулить строку - по выбранной номенклатуре будут обнулены все ячейки, отвечающие за подтвержденное количество во всех заказах
    - Сохранить заказ - сохраняет подтвержденное количество по выбранному заказу
    - Подтвердить заказ - переводит выбранный заказ в статус "Подтвержден", который указывается в настройках
    - Открыть заказ - открывает выбранный заказ для просмотра
    - Заказано -> Подтверждено - переносит количество из колонки "Заказано" в колонку "Подтверждено" для выбранного заказа

2. В командной панели

    - Сохранить - сохраняет подтвержденное количество по всем заказам
    - Подтвердить - переводит все заказы в статус "Подтвержден"
    - Заказано -> Подтверждено - переносит количество из колонки "Заказано" в колонку "Подтверждено" для всех заказов
    - Включить/Выключить компактный режим - скрывает/отображает колонки кратность, единицы измерения, заказано по заказам

[![9][9]][9]

Вносим подтвержденное количество товаров и нажимаем кнопку **"Сохранить"** для сохранения заказов, а затем **"Подтвердить"** для установки состояния - Заказ клиента подтвержден.

[![10][10]][10]

Заказы будут скорректированы согласно подтвержденному количеству, переходим к заказу на 29.05.2020 для контрагента "ООО "АШАН" и убеждаемся, что количество для этапа "Подтвержденный" будет равно подтвержденному в АРМе **"Формирование плана отгрузки"**, причина расхождений - Расхождения при отгрузке, а состояние - Заказ клиента подтвержден.

[![11][11]][11]

Редактировать количество заказываемого товара на разных этапах заказа можно также в заказе клиента, для этого необходимо переходить между этапами и менять количество товара в таблице, так же при внесении изменений можно указывать причину расхождений:

[![12][12]][12]

[![13][13]][13]

Для подтверждения заказов клиентов так же можно использовать регламентное задание, тогда подтвержденное количество, этап и состояние в заказах будут указываться автоматически. Автоматически  подтверждаются заказы для которых в настройках установлен признак "Использовать для автоматического подтверждения"

Подтверждение заказов клиентов осуществляется в соответствии с "Приоритетами подтверждения заказов", которые настраиваются в "Настройках исполнения заказов"

[![3][3]][3]

[![14][14]][14]

При настройке приоритетов указываются:

- Получатель - точка доставки
- Начало подтверждения - время, начиная с которого подтверждаются заказы
- Окончание подтверждения - время, начиная с которого перестают подтверждаться заказы
- Приоритет - для точек доставки с наибольшим приоритетом будут обеспечиваться заказы в первую очередь
- Утвержденные заказы - признак при установке которого заказы для точки доставки подтверждаются один раз и при повторном запуске регламентного задания не изменяются

[![15][15]][15]

За подтверждение заказов отвечает регламентное задание **"Автоматическое подтверждение заказов"**, для него можно настроить расписание или выполнить вручную.

[![16][16]][16]

[1]: 1.png
[2]: 2.png
[3]: 3.png
[4]: 4.png
[5]: 5.png
[6]: 6.png
[7]: 7.png
[8]: 8.png
[9]: 9.png
[10]: 10.png
[11]: 11.png
[12]: 12.png
[13]: 13.png
[14]: 14.png
[15]: 15.png
[16]: 16.png