# **![](https://habrastorage.org/webt/3v/u0/jo/3vu0joj9uqy1nxjnrgig42dx6s4.png)**

**[по-русски]**

Приложение **A-Explorer** является "клиентской частью" связки **A-Explorer + BRIDGE**. **BRIGDE** – скетч, который умеет работать с памятью **SPIFFS** (а так же **SD**, при внесении небольших изменений в код) он компилируется и загружается в память устройства. По последовательному порту происходит общение между связкой.

В самом начале сеанса передают флаг в виде одного символа. Таких основных флагов: **D** (скачать), **M** (память), **L** (список файлов), **R** (удалить), **E** (форматировать), **U** (загрузить), **X** (исполнить) и **Q** (перезагрузить). Далее передаются для каждого флага прочие параметры, такие как: размер имени файла, имя файла и т. д.

В функционал связки, нетрудно докадаться, включено получение списка всех файлов в памяти, получение информации о пространстве, удаление файлов, загрузка файлов в память устройства и скачака файлов с памяти, форматирование, исполнение устройством файла (например отображение изображения на ЖК-дисплее). В браузере файлов для каждого расширения назначена соотвествующая иконка. Прогресс загрузки отображается в процентах в статусбаре. Информация о занятом пространстве отображается в прогрессбаре.

**[English]**

**A-Explorer** app it's GUI for **BRIDGE**. **BRIDGE** – sketch and same name function inside can operate within **SPIFFS** memory (also **SD**, with a little code modification) will be compiled and flash to device.

In begin of session GUI sent one char flag. Main flags:  **D** (download), **M** (memory), **L** (list), **R** (remove), **E** (format), **U** (upload), **X** (execute) и **Q** (reboot). In next step sending any parametrs like as size of file, name of file and e. t. c.

It’s easy to prove that the bundle’s functionality includes a getting file list, space inforamtion, removing files, uploading and downloading, format memory, execution file (for example showing picture on LCD screen). In file browser shows percentage. Space of memory info show in progressbar.