---
title: Драйвери и фърмуер
---

Ние сме програмирали вместо Вас фърмуера. Трябва само да инсталирате драйверите и да копирате фърмуера на вашия NodeMCU (ESP8266).

За да комуникирате с вашия ESP8266, имате нужда от usb2serial драйвери за вашата операционна система.

Чипсетът за NocdeMCUs v3 обикновено е CH341, просто проверете на гърба на вашия NodeMCU, за да намерите някаква техническа информация.

Изберете връзката, която съответства на операционната система на вашия компютър.

### Windows

##### Драйвери за модел V2 (CP2102) за Windows
* [Windows 10](https://www.silabs.com/documents/public/software/CP210x_Universal_Windows_Driver.zip) - Windows 10 трябва да може да ги изтегля автоматично
* [Windows 7/8/8.1](https://www.silabs.com/documents/public/software/CP210x_Windows_Drivers.zip) - 32-bit версия за тези ОС, които не поддържат 64-bit версии

##### Драйвери за модел V3 (CH341) за Windows
* [Windows](http://www.wch.cn/downloads/file/5.html) - Windows 10 трябва да може да ги изтегля автоматично

##### Разархивирайте изтегления файл. Разархивирайте това:
* за V2: Отворете папката CP210x и кликнете два пъти върху приложението CP210xVCPInstaller_x64 (или x86)
* за V3: Отворете папката CH341SER и кликнете два пъти върху приложението SETUP.

---

### MacOS

#####  Драйвери за MacOS
* [NodeMCU V2](https://www.silabs.com/documents/public/software/Mac_OSX_VCP_Driver.zip )
* [NodeMCU V3](http://www.wch.cn/downloads/file/178.html) 

#####  Разархивирайте изтегления файл за MacOS.
* за V2: Разархивирайте папката CP210x и кликнете два пъти върху приложението CP210xVCPInstaller_x64 (or x86)
* за V3: Разархивирайте папката CH341SER и кликнете два пъти върху приложението SETUP.
* Рестартирайте своя Mac

---

### Linux
Няма драйвери за инсталиране. Чипът трябва да се поддържа директно (с проверими dmesg)

---
### Firmware Flasher 
Поддържа различни операционни системи: Windows, MacOS и Linux.

* [airRohr Flashing Tool](http://firmware.sensor.community/airrohr/flashing-tool/)
* [Изходен текст](https://github.com/opendata-stuttgart/airrohr-firmware-flasher)

Свържете NodeMCU към компютъра с къс микро USB кабел (кабелът не трябва да е по-дълъг от 1 м, в противен случай инсталацията може да се провали). Изберете `latest_bg.bin` (или друга езикова версия)и кликнете върху „Upload“.
Изчакайте, докато процесът приключи. Сега остава да сглобите станцията.
<br>
Голяма благодарност отива при [Piotr, from Poland](https://dropbox.inf.re/), за неговата помощ! 🙋‍♂️ 

