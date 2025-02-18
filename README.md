# Modular easy button screen for ESPHome + LVGL on cheap touchscreen devices

## Supported Devices
* Guition `ESP32-4848s040` 4.0" with capacitive touch and USB-C [AliExpress Link](https://www.aliexpress.us/item/3256806436431838.html).
* Guition `JC3248W535` 3.5" with capacitive touch and USB-C. [AliExpress Link](https://www.aliexpress.com/item/1005007566046827.html).
* Sunton `ESP32-2432S028R` 2.8" with resistive touch and USB micro-B. [AliExpress Link](https://www.aliexpress.com/item/1005004502250619.html).
* Sunton `ESP32-8048S043` 4.3" with capactivive touch and USB-C. [AliExpress Link](https://www.aliexpress.com/item/1005004788147691.html).
* Sunton `ESP32-8048S050` 5.0" with capactivive touch and USB-C. [AliExpress Link](https://www.aliexpress.com/item/1005004952694042.html).
* Elecrow CrowPanel `DIS05035H` (v2.2) 3.5" with resistive touch and USB-C. [Manufacturer's Link](https://www.elecrow.com/esp32-display-3-5-inch-hmi-display-spi-tft-lcd-touch-screen.html).

# Example ESPHome config files for screens and devices

I use a lot of svg vector graphics. The latest ESPHome does not install svg by default. Use pip to install cairosvg. 

```
pip install esphome cairosvg
```

### SDL Display on host

The SDL display platform allows you to use create an ESPHome display on a desktop system running Linux or MacOS. This is particularly useful for designing display layouts, since compiling and running a host binary is much faster than compiling for and flashing a microcontroller target system.

### `ESP32-4848s040` 4.0" 480px * 480px Smart Screen

This is a really great little screen.  guition-esp32-s3-4848s040-display_modular.yaml has a boot screen, a system for dimming the backligh at night and some basic buttons for controlling local and Home Assistant devices.
