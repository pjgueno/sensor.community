---
title: Драйвер та прошивка
---

Ми вже підготували прошивку. Вам потрібно лише встановити драйвери та прошити плати NodeMCU (ESP8266) та Teensy 4.0.

Для спілкування з вашим ESP8266 вам потрібні usb2serial драйвери для вашої операційної системи.

Набір мікросхем для NocdeMCUs v3 зазвичай становить CH341, просто перевірте задню частину вашого NodeMCU, щоб знайти якусь технічну інформацію. Виберіть посилання, яке відповідає операційній системі вашого комп’ютера.

### Windows

##### Драйвери для моделі V2 (CP2102) для Windows
* [Windows 10](https://www.silabs.com/documents/public/software/CP210x_Universal_Windows_Driver.zip) - Windows 10 повинна мати можливість їх автоматичного завантаження
* [Windows 7/8 / 8.1](https://www.silabs.com/documents/public/software/CP210x_Windows_Drivers.zip) - 32-розрядна версія - ** не ** підтримує 64-розрядну версію ОС

##### Драйвер для моделі V3 (CH341) для Windows
* [Windows](http://www.wch.cn/downloads/file/5.html) - Windows 10 повинна мати можливість автоматично завантажувати їх

##### Витягніть завантажений файл для Windows:
* для V2: Відкрийте папку CP210x і двічі клацніть на програмі CP210xVCPInstaller_x64 (або x86)
* для V3: відкрийте папку CH341SER і двічі клацніть на програмі SETUP.

---

### MacOS

##### Драйвери MacOS
* [NodeMCU V2](https://www.silabs.com/documents/public/software/Mac_OSX_VCP_Driver.zip )
* [NodeMCU V3](http://www.wch.cn/downloads/file/178.html) 

##### Витягніть завантажений файл для MacOS.
* для V2: розпакуйте папку CP210x і двічі клацніть на програмі CP210xVCPInstaller_x64 (або x86)
* для V3: розпакуйте папку CH341SER і двічі клацніть на програмі SETUP.
* Перезапустіть Mac

---

### Linux
Не потрібно встановлювати драйвери. Чіп повинен підтримуватися безпосередньо (перевіряється за допомогою dmesg)

---
### Прошивка NodeMCU
Підтримка декількох операційних систем: Windows, MacOS та Linux.

* [Інструмент прошивки airRohr](http://firmware.sensor.community/airrohr/flashing-tool/)
* [Вихідний код](https://github.com/opendata-stuttgart/airrohr-firmware-flasher)

Підключіть NodeMCU до комп’ютера за допомогою короткого кабелю micro-USB (виберіть один коротший за 1 метр, інакше установка може не вдатися). Виберіть `latest_en.bin` (або іншу мовну версію) і натисніть" Завантажити ".
Зачекайте, поки процес закінчиться. Тепер ми можемо зібрати датчик.
<br>
Велика подяка [Пьотру, з Польщі](https://dropbox.inf.re/), за допомогу! 🙋‍♂️

---
### Прошивка прошивки Teensy
У [Github Гельмута Біттера](https://github.com/hbitter/DNMS/tree/master/Firmware) ви можете знайти два типи прошивки:
* .я не
* .hex

##### Teensy Loader
Ви можете прошити файл .hex на платах Teensy за допомогою автономного програмного забезпечення графічного інтерфейсу [Teensy Loader](https://www.pjrc.com/teensy/loader.html) для Windows, Mac і Linux.
Також існує версія командного рядка.

##### Teensyduino
Ви можете прошити файл .ino на платах Teensy з розширенням IDE Arduino [Teensyduino](https://www.pjrc.com/teensy/teensyduino.html).
За потреби ви можете змінити прошивку безпосередньо в IDE Arduino.