---
title: Πρόγραμμα οδήγησης &amp; υλικολογισμικό
---

Έχουμε ήδη προετοιμάσει το υλικολογισμικό. Το μόνο που πρέπει να κάνετε είναι να εγκαταστήσετε τους οδηγούς και να φλασάρετε το NodeMCU (ESP8266).

Για να επικοινωνήσετε με το NodeMCU (ESP8266) χρειάζεστε usb2serial οδηγούς για το λειτουργικό σας σύστημα.

Το chipset για τα NocdeMCUs v3 είναι συνήθως το CH341, απλά ελέγξτε το πίσω μέρος του NodeMCU σας (ESP8266) για να βρείτε κάποιες τεχνικές πληροφορίες.

Επιλέξτε το σύνδεσμο που αντιστοιχεί στο λειτουργικό σύστημα του υπολογιστή σας.

### Windows

##### Οδηγούς για NodeMCU (ESP8266) V2 (CP2102) για Windows
* [Windows 10](https://www.silabs.comdocumentspublicsoftwareCP210x_Universal_Windows_Driver.zip) - Τα Windows 10 θα πρέπει να είναι σε θέση να κατεβάσουν αυτόματα αυτά τα προγράμματα.
* [Windows 788.1](https://www.silabs.comdocumentspublicsoftwareCP210x_Windows_Drivers.zip) - έκδοση 32-bit - **δεν** υποστηρίζει έκδοση 64-bit OS

##### Πρόγραμμα οδήγησης για NodeMCU (ESP8266) V3 (CH341) για Windows
* [Windows](http://www.wch.cndownloadsfile5.html) - Τα Windows 10 θα πρέπει να είναι σε θέση να τα κατεβάσουν αυτόματα.

##### Εξαγάγετε το αρχείο που κατεβάσατε για τα Windows:
* για NodeMCU (ESP8266) V2: Ανοίξτε το φάκελο CP210x και κάντε διπλό κλικ στην εφαρμογή CP210xVCPInstaller_x64 (ή x86)
* για NodeMCU (ESP8266) V3: ανοίξτε το φάκελο CH341SER και κάντε διπλό κλικ στην εφαρμογή SETUP.

---

### MacOS

##### Οδηγούς MacOS
* [NodeMCU V2](https://www.silabs.comdocumentspublicsoftwareMac_OSX_VCP_Driver.zip )
* [NodeMCU V3](http://www.wch.cndownloadsfile178.html)

##### Εξαγάγετε το αρχείο που κατεβάσατε για MacOS.
* για το V2: και κάντε διπλό κλικ στην εφαρμογή CP210xVCPInstaller_x64 (ή x86).
* για V3: Αποσυμπιέστε το φάκελο CH341SER και κάντε διπλό κλικ στην εφαρμογή SETUP.
* Επανεκκίνηση του Mac σας

---

### Linux
Δεν χρειάζεται να εγκατασταθούν προγράμματα οδήγησης. Το τσιπ θα πρέπει να υποστηρίζεται άμεσα (επαληθεύεται με το dmesg)

---
### Firmware Flasher
Υποστήριξη πολλαπλών λειτουργικών συστημάτων: Windows, MacOS και Linux.

* [airRohr Flashing Tool](http://firmware.sensor.communityairrohrflashing-tool)
* [Πηγαίος κώδικας](https://github.comopendata-stuttgartairrohr-firmware-flasher)

Συνδέστε το NodeMCU στον υπολογιστή σας με ένα κοντό καλώδιο micro-USB (επιλέξτε ένα καλώδιο μικρότερο από 1 μέτρο, διαφορετικά η εγκατάσταση μπορεί να αποτύχει). Επιλέξτε `latest_en.bin` (ή μια άλλη γλωσσική έκδοση) και κάντε κλικ στο "Upload".
Περιμένετε μέχρι να ολοκληρωθεί η διαδικασία. Τώρα μπορούμε να συναρμολογήσουμε τον αισθητήρα.

#### Linux: Ορισμός δικαιωμάτων ως εκτελέσιμο
Μετά τη λήψη μπορεί να χρειαστεί να ορίσετε την άδεια εκτέλεσης. Αυτό μπορεί να γίνει με την εντολή: `chmod o+x <όνομα αρχείου λήψης>`
<br>
Ένα μεγάλο ευχαριστώ στον [Piotr, από την Πολωνία](https://dropbox.inf.re), για τη βοήθειά του! 🙋♂️

#### MacOS: πώς να εκτελέσετε μια ανεπιβεβαίωτη εφαρμογή
Κάντε δεξί κλικ και ανοίξτε την εφαρμογή αρκετές φορές και επιβεβαιώστε πάντα με "Άνοιγμα".

Εδώ είναι ένα σύντομο βίντεο στο Youtube 👉 https://youtu.be1KZiP94TYjw




