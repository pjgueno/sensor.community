---
title: Driver & firmware
---

We already prepared the firmware. You only have to install drivers and flash your NodeMCU (ESP8266) and Teensy 4.0 boards. 

To communicate with your ESP8266 you need usb2serial drivers for your operating system. 

The chipset for NocdeMCUs v3 is usually CH341, just check the back of your NodeMCU to find some technical information. Choose the link that corresponds to the operating system of your computer.

### Windows

##### Drivers for model V2 (CP2102) for Windows
* [Windows 10](https://www.silabs.com/documents/public/software/CP210x_Universal_Windows_Driver.zip) - Windows 10 should be able to automatically download these
* [Windows 7/8/8.1](https://www.silabs.com/documents/public/software/CP210x_Windows_Drivers.zip) - 32-bit version - **not** supporting 64-bit version OS

##### Driver for model V3 (CH341) for Windows
* [Windows](http://www.wch.cn/downloads/file/5.html) - Windows 10 should be able to automatically download these

##### Extract the downloaded file for Windows:
* for V2: Open the folder CP210x and double click on the application CP210xVCPInstaller_x64 (or x86)
* for V3: open the folder CH341SER and double click on the application SETUP.

---

### MacOS

#####  MacOS Drivers
* [NodeMCU V2](https://www.silabs.com/documents/public/software/Mac_OSX_VCP_Driver.zip )
* [NodeMCU V3](http://www.wch.cn/downloads/file/178.html) 

#####  Extract the downloaded file for MacOS.
* for V2: Unzip the folder CP210x and double click on the application CP210xVCPInstaller_x64 (or x86)
* for V3: Unzip the folder CH341SER and double click on the application SETUP.
* Restart your Mac

---

### Linux
No drivers need to be installed. Chip should be supported directly (verifiable with dmesg)

---
### Firmware Flasher NodeMCU
Support for multiple Operating Systems: Windows, MacOS and Linux.

* [airRohr Flashing Tool](http://firmware.sensor.community/airrohr/flashing-tool/)
* [Source Code](https://github.com/opendata-stuttgart/airrohr-firmware-flasher)

Connect NodeMCU to your computer with a short micro-USB cable (choose one shorter than 1 Meter, otherwise the installation may fail). Select `latest_en.bin` (or another language version) and click “Upload”.
Wait until the process is done. Now we can assemble the sensor.
<br>
A big thanks goes to [Piotr, from Poland](https://dropbox.inf.re/), for his help! 🙋‍♂️ 

---
### Firmware Flasher Teensy
In [Helmut Bitter's Github](https://github.com/hbitter/DNMS/tree/master/Firmware) you can find two kinds of firmware: 
* .ino
* .hex

#####  Teensy Loader
You can flash the .hex file in the Teensy boards with the standalone GUI software [Teensy Loader](https://www.pjrc.com/teensy/loader.html) for Windows, Mac and Linux.
A command line version also exist.

#####  Teensyduino
You can flash the .ino file in the Teensy boards with the Arduino IDE extension [Teensyduino](https://www.pjrc.com/teensy/teensyduino.html).
If needed, you can modify the firmware directly in the Arduino IDE.