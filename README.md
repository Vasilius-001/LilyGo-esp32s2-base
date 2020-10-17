# LILYGO® TTGO T8 ESP32-S2 V1.1 WIFI Wireless Module Type-C Connector TF Card Slot Development Board

###Product Description

Hardware Specifications
-----------------------
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


1. Before using this project, please set up the esp-idf environment, specific reference [esp-idf-docs](https://docs.espressif.com/projects/esp-idf/en/latest/esp32s2/get-started/index.html)
2. Clone the project and then allow `idf.py build`
3. Use `idf.py -p [your port] -b 115200 flash` to download to the board


### Information for new users:
- If you have an SD card, please open this definition in app_main.c 49 line
    ```
    // #define HAS_SDCARD       //If you have an SD card, please open this definition
    ```
- IO14 is connected to the SD card of the board, and the power of the LED controls the IO Pin. When you use the battery, you need to set IO14 to high level to use the SD card.



