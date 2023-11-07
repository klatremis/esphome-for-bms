# esphome-for-bms
Two solutions
* DIY generic esp32 & TTL converter hardware, use "seplos-esp32" and the wiring below
* For KlatremisHW/Lilygo, use "seplos-klatremishw" file

## Supported hardware
Seplos BMS
* Multiple or standalone Seplos BMS 2.0 V16 (with CAN to master, the master cant be monitored this way over rs485)

## Requirements
* ESP32
* TTL To RS485 Module with automatic flow control  
or  
* KlatremisHW Basic/Lilygo t-can 485, *For now, only danish customers: https://badenergy.dk/product-category/inverter/inverter-styring/

## KlatremisHW solution example
 ![image](https://github.com/klatremis/esphome-for-bms/blob/main/klatremishw.jpg)

## All sensors in Home assistant
![image](https://github.com/klatremis/esphome-for-bms/blob/main/all_sensors.png)

## Lovelace dashboard example
Thanks to PVPRO/Jonas for the below dashboard example <3 Link to his page about it: https://github.com/pvprodk/HA-seplos-bms

This example can be found in the files above (lovelace_dashboard.yaml)
#### HACS addon requirements
* custom:button-card
* custom:bar-card
* custom:apexcharts-card


![image](https://github.com/klatremis/esphome-for-bms/blob/main/lovelace_dashboard.png)

## Wiring of generic esp32 & TTL module
RX / TX between esp and ttl converter may have to be swapped. This seems to be a little different from espboard to espboard.
If it dosent communicate(RX/TX led both blinking) Try swap rx/tx on the esp.
 ![image](https://github.com/klatremis/esphome-for-bms/blob/main/wiring.jpg)
