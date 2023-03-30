**Учетные точки**
=================

Настройка всех интерфейсов, через которые ведется оперативный учет на
участке нормализации, происходит через справочники "Учетные точки" и
"Кнопки учетных точек".


**Справочник "Учетные точки".** 

Данный справочник используется для того,
чтобы отделить наборы операций, выполняемых на разных участках
производства. Например, логично отделить операции, связанные с выпусками
на этапе нормализации, от операций, связанных с выпусками на этапе заквашивания.  
При этом, если на предприятии на один только участок нормализации
ставится несколько сенсорных киосков (в ключевых точках - отдельно около
счетчика выпущенной смеси, отдельно около переданной смеси в
танки заквашивания и тп), то разумно на каждый киоск сделать отдельную
учетную точку, пусть и  с одной операцией.
 

 

-   Открыть справочник "Учетные точки" и перейти к созданию нового элемента:  
![](AccountPoints.assets/drex_uchetnye_tochki_2_custom.png)
-   Указать наименование:  
![](AccountPoints.assets/drex_uchetnye_tochki_2_custom_2.png)
-   Указать список пользователей, у которых будет доступ к этой учетной
    точке (т.е. только они смогут выполнять операции, относящиеся к этой
    учетной точке):  
![](AccountPoints.assets/drex_uchetnye_tochki_2_custom_3.png)  
![](AccountPoints.assets/drex_uchetnye_tochki_2_custom_4.png)
-  Нажать "Записать и закрыть".


**Справочник "Кнопки учетных точек".**  

Данный справочник используется для того, чтобы настраивать различные операции, выполняемые на определенном участке производства. Например, для этапа нормализации логично выделить кнопку для выпуска смеси, еще, возможно, для её передачи на заквашивание.
     
-   Открыть справочник "Учетные точки". Среди списка найти нужную,
    открыть:  
![](AccountPoints.assets/drex_uchetnye_tochki_2_custom.png)
-   В таблице кнопок нажать "Создать":  
![](AccountPoints.assets/drex_uchetnye_tochki_2_custom_5.png)
-   Указать наименование и выбрать обработку "Работа с заданиями" - если
    выпуск смеси идут строго по заданию на смену или "Оперативный учет
    на рабочем центре" - в противном случае:  
![](AccountPoints.assets/drex_uchetnye_tochki_2_custom_6.png)
-   Указать в создаваемых документах "Переработка" и что при её создании
    нет списания материалов:  
![](AccountPoints.assets/drex_uchetnye_tochki_2_custom_7.png)
-   Указать видимость кнопки выпуска и что не ведется учет по таре:  
![](AccountPoints.assets/drex_uchetnye_tochki_2_custom_8.png)
-   Указать участок нормализации:  
![](AccountPoints.assets/drex_uchetnye_tochki_2_custom_9.png)
-   Ограничить склады для выпуска:  
![](AccountPoints.assets/drex_uchetnye_tochki_2_custom_10.png)
-   Нажать "Записать и закрыть".

 

Более подробная информация о параметрах кнопок учетных точек описана в
разделе ["Кнопки учетных точек"](../../../CommonInformation/Handbooks/ButtonOfAccountPoint/readme.md).