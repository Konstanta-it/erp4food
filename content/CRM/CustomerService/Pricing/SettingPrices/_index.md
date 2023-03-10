---
title: "Установка цен"
draft: false
weight: 3
---

Для установки ценового значения на [вид цены](https://konstanta-it.github.io/erp4food/CRM/CustomerService/Pricing/TypesOfPrices) используется документ **"Установка цен"**, который расположен в разделе **"Заказы"** в подсистеме **"Цены и скидки"** - **"История изменения цен"**.

![1](1.png)

При создании документа **"Установка цен"** на первой странице **Выбор видов цен** необходимо заполнить:

- Номер (заполняется автоматически)
- Дата документа
- Номер за день (заполняется автоматически), если на этот день уже создан документ установки цен
- Виды цен по которым будет проводиться установка (достаточно выбрать базовый вид цены - зависимые от него виды цен при установке подтянутся автоматически)
- Ответственный
- Комментарий

Создадим документ установки цен на 27.05.2020 для Базового вида цены, зависимые от него виды цен подтянутся автоматически:

![2](2.png)

Далее необходимо нажать на кнопку **"Перейти к установке цен"**

![3](3.png)


Откроется вторая страница документа, на ней добавляются номенклатурные позиции на которые устанавливаются цены. Подбор номенклатуры возможен с помощью быстрых отборов и поиска.

Для номенклатуры по каждому выбранному виду цен автоматически заполняется текущая цена. Новая цена может быть заполнена вручную или автоматически с помощью кнопки **"Изменить цены"** - **"Заполнить текущую цену по актуальной"**. После заполнения новую цену можно увеличивать или уменьшать на %  с помощью кнопок **"Изменить цены"** - **"увеличить цены, %"** и **"уменьшить цены, %"**.

По кнопке **"Обмен"** можно загружать цены из табличного документа.

Установим цену для номенклатур Сыр Костромской, Сыр Адыгейский и Сыр Пошехонский, задав ценовые значения вручную как показано на картинке:

![4](4.png)

Сохраняем документ, для этого нажимаем кнопку **"Провести и закрыть"**.

![5](5.png)
