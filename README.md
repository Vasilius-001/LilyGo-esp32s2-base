# LILYGO® TTGO T8 ESP32-S2 V1.1

WIFI Wireless Module Type-C Connector TF Card Slot Development Board

<img align="cener" width=400 src="Images/LilyGO_esp32s2_T8_v1.1-6.jpg" /><img align="cener" width=400 src="Images/LilyGO_esp32s2_woor_T8_v1.1-6.jpg" />

### Product Description

Hardware Specifications||
-----------:|:------------
Chipset|ESPRESSIF-ESP32-S2
FLASH|4MB 
PSRAM|8MB
SRAM|320 kB SRAM
Button|Power Switch,Rest,Boot,Customize,DPI Switch
External Device|TF Card
USB to TTL|CH340C
Modular interface|SD card、UART、SPI、I2C、PWM、I2S、ADC
On-board clock|32.768KHz crystal oscillator 
Working voltage|2.7V-3.6V
Working temperature range|-40℃ ~ +85℃
Weight|7g
Size|65.21*25.95*5mm
**Power Supply**||
Power Supply Input|USB 5V/1A
Charging current|500mA
Battery Input|3.7-4.2V
JST Connector|2Pin 1.25mm
USB|Type-C USB
**Wi-Fi**||
Standard|FCC/CE-RED/IC/TELEC/KCC/SRRC/NCC(esp32 chip)
Protocol|802.11 b/g/n(802.11n，speed up to150Mbps)A-MPDU and A-MSDU polymerization，support 0.4μS Protection interval
Frequency range|2.4GHz-2.5GHz(2400M-2483.5M)
Transmit Power|22dBm
Communication distance|300m

## Таблица выводов

<img align="cener" width=400 src="Images/LilyGO_esp32s2_T8_v1.1-Pinmap.jpg" /><img align="cener" width=400 src="Images/LilyGO_esp32s2_woor_T8_v1.1-Pinmap.jpg" />

## Размеры

<img align="cener" width=400 src="Images/LilyGO_esp32s2_T8_v1.1-Dimension.png" /><img align="cener" width=400 src="Images/LilyGO_esp32s2_woor_T8_v1.1-Dimension.png" />

## More Information

https://github.com/Xinyuan-LilyGO/LilyGo-esp32s2-base

## Програмное обеспечение

1. Перед использованием этого проекта настройте среду ESP-IDF, конкретную ссылку [esp-idf-docs](https://docs.espressif.com/projects/esp-idf/en/latest/esp32s2/get-started/index.html)
2. Клонируйте проект, а затем выполните `idf.py build`
3. Используйте `idf.py -p [ваш порт] -b 115200 flash` для загрузки на плату


### Информация для новых пользователей:
- Если у вас есть SD-карта, откройте это определение в app_main.c строка 49
    ```
    // #define HAS_SDCARD       //If you have an SD card, please open this definition
    ```
- Вывод IO14 подключен к SD-карте платы, управление питанием светодиода - вывод IO. Когда вы используете аккумулятор, вам необходимо установить на выводе IO14 высокий уровень, чтобы использовать SD-карту.



