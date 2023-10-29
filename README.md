# esphome-for-bms
For DIY generic esp32 hardware, use "seplos-esp32" and the wiring below
For KlatremisHW, use "seplos-klatremishw" file

## Supported hardware
Seplos BMS
* Multi Seplos BMS 2.0 V16

## Requirements
* ESP32
* TTL To RS485 Module with automatic flow control
or
* KlatremisHW/Lilygo t-can 485, *For now only danish customers: https://badenergy.dk/product-category/inverter/inverter-styring/

## Home Assistant dashboard sensors example
 ![image](https://github.com/klatremis/esphome-for-bms/blob/main/dashboard.jpg)

## Wiring of generic esp32 & TTL module
RX / TX between esp and ttl converter may have to be swapped. This seems to be a little different from espboard to espboard.
If it dosent communicate(RX/TX led both blinking) Try swap rx/tx on the esp.
 ![image](https://github.com/klatremis/esphome-for-bms/blob/main/wiring.jpg)

