---
title: Ovladače & firmware
---

Firmware je pro Vás už připraven. Musíte si pouze nainstalovat drivery a nahrát firmware do Vašich modulů NodeMCU (ESP8266) a Teensy 4.0.

Ke komunikaci mezi ESP8266 a Vaším operačním systémem je zapotřebí nainstalovat usb2serial drivery.

NodeMCU v3 chipset je obvykle CH341, zkontrolujte zadní stranu Vašeho NodeMCU pro další informace. Vyberte odkaz, který odpovídá operačnímu systému vašeho počítače.

### Windows

##### Ovladač modelu V2 (CP2102) pro Windows
* [Windows 10](https://www.silabs.com/documents/public/software/CP210x_Universal_Windows_Driver.zip) - Windows 10 by měly být schopny tyto drivery automaticky stáhnout.
* [Windows 7/8/8.1](https://www.silabs.com/documents/public/software/CP210x_Windows_Drivers.zip) - 32-bitová verze - **nepodporuje** 64-bitovou verzi Windows.

##### Ovladač modelu V3 (CH341) pro Windows
* [Windows](http://www.wch.cn/downloads/file/5.html) - Windows 10 by měly být schopny tyto drivery automaticky stáhnout.

##### Rozbalte stažený soubor pro Windows:
* pro V2: Otevřete adresář CP210x a dvojklikem spusťte soubor CP210xVCPInstaller_x64 (or x86)
* pro V3: Otevřete adresář CH341SER a dvojklikem spusťte soubor SETUP.

---

### MacOS

#####  MacOS Ovladače
* [NodeMCU V2](https://www.silabs.com/documents/public/software/Mac_OSX_VCP_Driver.zip )
* [NodeMCU V3](http://www.wch.cn/downloads/file/178.html)

#####  Rozbalte stažený soubor pro MacOS.
* pro V2: Otevřete adresář CP210x a dvojklikem spusťte soubor CP210xVCPInstaller_x64 (or x86)
* pro V3: Otevřete adresář CH341SER a dvojklikem spusťte soubor SETUP.
* Restarujte Váš Mac

---

### Linux
Nemusíte instalovat žádné ovladače. Chip by měl být podporovaný přímo. (můžete zkontrolovat s dmesg)

---
### Nástroj na instalaci firmware NodeMCU
Podporuje vícero operačních systémů: Windows, MacOS and Linux.

* [airRohr Flashing Tool](http://firmware.sensor.community/airrohr/flashing-tool/)
* [Zdrojový kód](https://github.com/opendata-stuttgart/airrohr-firmware-flasher)

Připojte k počítači modul NodeMCU pomocí krátkého micro-USB kabelu (kabel by měl být kratší než 1 metr, jinak může instalace selhat). Vyberte `latest_en.bin`  (nebo jiný jazyk) a klikněte na “Nahrát”. Počkejte na dokončení procesu nahrávání. Teď můžete pokračovat k samotnému složení senzoru.
<br>
Velký dík patří [Piotrovi, z Polska](https://dropbox.inf.re/), za jeho pomoc! 🙋‍♂️

---
### Nástroj na instalaci firmware Teensy
Na [Githubu Helmuta Bittera](https://github.com/hbitter/DNMS/tree/master/Firmware) můžete najít dva typy firmware:
* .ino
* .hex

#####  Teensy Loader
Soubor .hex můžete flashovat na desku Teensy pomocí samostatného softwaru GUI [Teensy Loader](https://www.pjrc.com/teensy/loader.html) dostupný pro Windows, Mac a Linux.
Existuje také verze pouze s příkazovým řádkem.

#####  Teensyduino
Soubor .ino můžete flashovat na desku Teensy pomocí rozšíření Arduino IDE [Teensyduino](https://www.pjrc.com/teensy/teensyduino.html).
V případě potřeby můžete firmware upravit přímo zde v Arduino IDE.
