---
title: Вступление
---
 
  <div class="max-w-screen-xl mx-auto pb-5">
    <div class="p-2 rounded-lg bg-indigo-100 shadow-lg sm:p-3">
    <div class="flex items-center">
          <span class="p-2 rounded-lg bg-indigo-500">
            <svg class="h-8 w-8 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11 5.882V19.24a1.76 1.76 0 01-3.417.592l-2.147-6.15M18 13a3 3 0 100-6M5.436 13.683A4.001 4.001 0 017 6h1.832c4.1 0 7.625-1.234 9.168-3v14c-1.543-1.766-5.067-3-9.168-3H7a3.988 3.988 0 01-1.564-.317z" />
            </svg>
          </span>
        <div class="flex-wrap flex">
          <p class="pt-1 text-indigo-700 font-medium">
              Сенсор звука пока в статусе бета. Задавайте вопросы на  <a href="https://forum.sensor.community/" target="_blank">forum.sensor.community</a>  или почту </p>
        <a href="mailto:Noise@Sensor.Community" class="ml-1 font-medium underline text-white hover:text-yellow-600">
                Noise@Sensor.Community</a>
        </div>
    </div>
  </div>
</div>

<br>

> 🚧 Sensor.Community это всемирная сеть сенсоров окружающей среды информация с которых доступна в виде открытых данныех. Соберите свою станцию измерения и присоединяйтесь к сети Sensor.Community! С сенсором DNMS (от английского Digital Noise Measuring Sensor) вы сможете измерять также и шумовое загрязнение.

 <img src="../docs/dnms/dnms-noise-measuring-sensor-kit.jpg" style="display: block; margin: 1em 0" loading="lazy"/>


Ознакомиться с оригинальном инструкций и предыдущими версиями датчика шума можно в [GitHub'е Хельмута Биттера](https://github.com/hbitter/DNMS/tree/master/Manual).

<br>

В этом репозитории содержатся варианты сборки датчика с использованием разных печатных плат.
 
 <br>
 
 Существует два варианта сборки:
 
* сборка, при которой контроллер NodeMCU с сенсорами (PM, температура, влажность и т.д.) и DNMS раздельны. Печатные платы, соответсвенно, называются AIRROHR V1.4 и DNMS - T4 V1.4.
* комбинированная версия, где контроллер NodeMCU и DNMS размещены на одной печатной плате. Такой вариант называется DNMS-T4 + NodeMCU V1.4.
 
В данном руководстве описан только первый вариан с раздельными платами. В этом случае длина соединения между NodeMCU и DNMS может достигать 10 метров, что важно, так как для получения точных измерений шума необходимо найти правильноe место для установки сенсора звука DNMS.
Второй вариант описан в [GitHub'е Хельмута Биттера](https://github.com/hbitter/DNMS/tree/master/Manual).

### Список покупок

##### Компоненты сенсора шума DNMS
Компонент | Описание | Ссылки на продавцов
------------ | -------------  | -------------
ESP8266 NodeMCU v3 <img src="https://www.cytron.io/image/cache/catalog/products/NODEMCU-V3/NodeMCU%20V3%20Lolin%20(1)-800x800.jpg" width="100" height="100" loading="lazy"/> | процессор с возможностью подключения к WiFi. Версия NodeMCU v2 не рекомендуется к покупке, также как и платы без металлической защиты от помех на чипе WiFi | [проверенный продавец](https://ru.aliexpress.com/item/5pcs-lot-New-Wireless-module-NodeMcu-Lua-WIFI-Internet-of-Things-development-board-based-ESP8266-with/32266751149.html) <br /> [список продавцов](https://www.aliexpress.com/wholesale?minPrice=&maxPrice=&isBigSale=n&isFreeShip=y&isNew=n&isFavorite=n&shipFromCountry=&shipCompanies=&SearchText=nodemcu+v3+esp8266+ch340&CatId=202001107&g=y&SortType=price_asc&needQuery=y) 
плата разработки Teensy 4.0 <img src="https://forum.pjrc.com/teensy40_front.jpg" width="100" height="100" loading="lazy"/> | Плата Teensy 4.0, оснащенная процессором NXP iMXRT1062 с ядром ARM Cortex-M7 с частотой 600 МГц, является самым быстрым микроконтроллером на сегодняшний день.  | [PJRC](https://www.pjrc.com/store/teensy40.html) <br /> [EXPTECH](https://www.exp-tech.de/plattformen/teensy/9596/teensy-4.0-development-board) <br /> [Antratek](https://www.antratek.de/teensy-4-0) <br /> [PIMORONI](https://shop.pimoroni.com/products/teensy-4-0-development-board)
Микрофон ICS-43434 <img src="https://cdn.tindiemedia.com/images/resize/zZfcH1YGwpqKUPjaCqdjy_y9bVg=/p/full-fit-in/1782x1336/i/44691/products/2017-07-15T04%3A32%3A01.633Z-ICS43434.top.jpg" width="100" height="100" loading="lazy"/> | цифровой микрофон с выходом I²S. | [tindie.com](https://www.tindie.com/products/onehorse/ics43434-i2s-digital-microphone/) 
Провода для подключения микрофона | Ультрагибкие силиконовые кабели диаметром 0,15 мм² (AWG 26) шести различных цветов | можно приобрести в местном магазине

К сенсору шума DNMS стоит также добавить компоненты для сборки сенсора твердых частиц, которые перечислены в отдельном [руководстве](https://sensor.community/ru/sensors/airrohr#Spisok_pokupok). Стоит заметить, что второй контроллер NodeMCU вам в этом случае не потребуется.


<br>

🙌 Отлично, что вы решили купить запчасти для собственной станции! 
К сожалению, доставка может занять от нескольких дней до месяца. 
А до тех пор наслаждайтесь жизнью :)
