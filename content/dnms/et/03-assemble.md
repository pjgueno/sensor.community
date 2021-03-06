---
title: Koosta
---
> ⚠️ **OLULINE MÄRKUS**
Enne kokkupanekut paigaldage püsivara!
Vt __firmware flasher__ jagu.


### Mikrofoniüksus

Mikrofoniüksus põhineb Pesky Products Breakout-plaadil koos MEMS-mikrofoniga ICS-43434. Sellist tahvlit saab osta [Tindie marketplace](https://www.tindie.comproductsonehorseics43434-i2s-digital-microphone).

Mikrofoniüksus põhineb Pesky Products Breakout-plaadil koos MEMS-mikrofoniga ICS-43434. Sellist tahvlit saab osta [Tindie marketplace](https://www.tindie.comproductsonehorseics43434-i2s-digital-microphone).


##### Mikrofoniüksuse korpus
Korpus on valmistatud .500" (12,7 mm) polüstüreenist torudest. See läbimõõt võimaldab ühendada otse enamik kalibraatoreid seadme külge.

Prototüüp töötati välja [Evergreen nr 236 torustikuga] (https://evergreenscalemodels.comproducts236-500-12-7mm-od-white-polystyrene-tubing).

Prototüüp töötati välja [Evergreen nr 236 torustikuga] (https://evergreenscalemodels.comproducts236-500-12-7mm-od-white-polystyrene-tubing).
<br>
Väljalülitusplaat tuleb viiluga kohandada torude läbimõõdule. Mikrofoni sisselaskeava kaitsmiseks kasutage teipi.
<br>

<br>
<br>

Seejärel joota kuus silikoonkaablit. Pange tähele, millise viiguga on kaabel ühendatud!

Seejärel joota kuus silikoonkaablit. Pange tähele, millise viiguga on kaabel ühendatud!
Lõika 115 mm pikkune torutükk.
<br>
Kleepige mikrofoniplaat ristatud teibiga. Pange kaablid torusse ja kinnitage plaat toru otsa.
<br>
<br>
<br>

Tee toru otsad teibiga tihedalt kinni.

Tee toru otsad teibiga tihedalt kinni.

Nüüd võite täita toru vaiguga. See samm on kohustuslik, et vältida resonantsi ning saada kalibreeritud ja reprodutseeritavaid andmeid.

Prototüüp töötati välja Copaltec GmbH toodetud [PURe Isolation ST 33](https://www.buerklin.comenPolyurethane-cast-resin-black-Copaltec-PURe-Isolation-ST-33p12L5900) abil.

##### Spetsifikatsioonid:
* Dielektriline tugevus: 28 kVmm
* Spetsiifiline edasine vastupanu: 5,8.1014 ohmcm
* Pinnatakistus: 1,3.1016 oomi
* Segamissuhe vaiguhapnik: 2 : 1
* Keeduaeg: 20 kuni 30 min.
* Kuivamisaeg: 16 kuni 30 tundi
* Lõplik kõvenemine: 10 kuni 14 päeva.
* Viskoossus (segatud): 500 kuni 600 mPa.s
* Shore kõvadus: D 50 kuni 55 (ISO 868, DIN 53505).
* Soojusjuhtivus: 0,3 WmK
* Rakendustemperatuurid: - 20 kuni +130 °C


Electrolube'i valmistatud [polüuretaanvaik UR5545](https://electrolube.comwp-contentuploads201911044-UR5545A-SDS1525.pdf) peaks samuti toimima.

Igale torule peaks piisama 15 g vaigust.

<img src="..docsdnmsdnms-müra-mõõtmine-mikrofoni-sisene-toru.jpg" style="display:block; margin: 2em 0" loading="lazy">

Kui vaik on kõvenenud, eemaldage teip. Teie mikrofon on valmis.



### DNMS korpus

Kui Teensy (DNMS) ja NodeMCU (eraldiseisev või trükkplaadil) on eraldatud: DNMS ja airRohr

Vaja on 25 mm läbimõõduga torutükki (näiteks elektripaigaldiste jaoks mõeldud torud), pistikut, 90° vibu ja M25 IP68 kaablifiltrit.

Toru ise peaks olema 160 mm pikk. DNMS näeb välja koht. Mikrofoni korpus säilib kaabli tihendiga.

Vibu takistab vee ja niiskuse sisenemist korpusesse, lastes samal ajal kaabli läbi.

<img src="..docsdnmsdnms-müra-mõõtmine-korpus.jpg" style="margin: 1em 0" loading="lazy">

DNMS on ühendatud teise trükkplaadiga RJ12 kaabli abil. Kui see kaabel on pikem kui 250 mm, tuleb kasutada I²C-pikendust.

<img src="..docsdnmsdnms-noise-measuring-sensor-kit.jpg" style="margin: 1em 0" loading="lazy">

Kui kõik on hästi ühendatud, liimitakse osad kokku.

Tulemus:

<img src="..docsdnmsdnms-noise-measuring-dn40-result.jpg" style="margin: 1em 0" loading="lazy">

NodeMCU-d sisaldava trükkplaadi võib paigutada ükskõik millisesse elektrikarpi.


### Ilmakaitse

Korpused ise peaksid olema veekindlad. Ainult mikrofoni sisselaskeava võiks olla tundlik. Tootja TDK on avaldanud mõned soovitused InvenSense'i alumiste MEMS-mikrofonide tihendamiseks tolmu ja vedeliku sissetungi eest, kuid komponente on raske leida ja neid ei ole testitud.

Ilmastikukaitse paigaldamine vahtkatte kujul on hädavajalik. Vajaduse korral piisab isegi kodusest käsnast. Selleks on mitu põhjust:
* see kaitseb tuulemüra eest (mis võib suurendada detsibellimõõtmisi).
* see kaitseb mikrofoni otsese vee lekke eest. Mikrofoni kondenseerumise vältimiseks tõmmake kate pärast selle paigaldamist veidi tagasi, et tekiks väike õõnsus.
* see kaitseb päikesekiirguse eest. Intensiivne päikesekiirgus võib mõjutada mõõteväärtusi ja vähendada mikrofoni eluiga.

* see kaitseb päikesekiirguse eest. Intensiivne päikesekiirgus võib mõjutada mõõteväärtusi ja vähendada mikrofoni eluiga.

Neid vahtkummi katteid müüakse tavaliselt kui "mõõtmismikrofonide katteid". Kuid need on kallid. Võid võtta ka tavalise vahtpalli ja lõigata kääridega augu sisse.

If you need more ones [this source](https://de.aliexpress.comitem32357483926.html?gps-id=pcStoreJustForYou&amp;scm=1007.23125.137358.0&amp;scm_id=1007.23125.137358.0&amp;scm-url=1007.23125.137358.0&amp;pvid=6cc8dfcd-974e-4fde-9dc9-6444c37a9069&amp;spm=a2g0o.store_home.smartJustForYou_148437547.2) can be helpful.

### Mikrofoni asukoht

Oluline on paigutada mikrofon võimalikult "vabale" kohale, see tähendab, et võimalikult väheste heli peegeldavate pindadega kohta. Kaugus peegeldavatest pindadest peaks olema võimalikult suur. Püüdke mitte paigaldada mikrofoni otse maja seinale, sest seinad peegeldavad helisid tugevasti.  Ideaalis peaks vahemaa seinast olema üle 1 m. Muidugi ei ole seda alati lihtne realiseerida.

Kui mikrofoni otsa ja seina vaheline kaugus on umbes 50 cm, on indutseeritud viga siiski mõistlik. Head kohad on näiteks rõdud või terrassipiirded või väike mast katusel.

Võite proovida paigutada mikrofoni ka otse maja nurka, et peegeldused osaliselt üksteist neutraliseeriksid.

Vabalt seisev, vähemalt 1 m kõrgune mast võiks samuti olla lahendus, kuid siis tuleb jälgida peegeldusi maapinnal. See sõltub muidugi põrandakattest.

Samuti on oluline olla alati teadlik sellest, et me mõõdame ümbritsevat müra.  Me saame ainult ligikaudselt hinnata selliste müraallikate nagu maantee või raudtee müra.

Mida lähemale te aga allikale lähete, seda täpsemaks muutub viide allikale. Firmware uuendamine peaks siis võimaldama saada täpsed mõõtmised tuvastatud tüüpi müra jaoks.

Mida lähemale te aga allikale lähete, seda täpsemaks muutub viide allikale. Firmware uuendamine peaks siis võimaldama saada täpsed mõõtmised tuvastatud tüüpi müra jaoks.
Mida lähemale te aga allikale lähete, seda täpsemaks muutub viide allikale. Firmware uuendamine peaks siis võimaldama saada täpsed mõõtmised tuvastatud tüüpi müra jaoks.
<br>
<br>
