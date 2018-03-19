# NodeMCU API
| Module | esp8266 | esp32 | linux | Description |
| --- | --- | --- | --- | -- |
| **adc** | supported | supported | - | The ADC module provides access to the in-built ADC. |
| **ads1115** | supported | - | - | This module provides access to the ADS1115 16-Bit analog-to-digital converter. |
| **adxl345** | supported | - | - | This module provides access to the [ADXL345](https://www.sparkfun.com/products/9836) triple axis accelerometer. |
| **am2320** | supported | - | - | This module provides access to the [AM2320](https://akizukidenshi.com/download/ds/aosong/AM2320.pdf) humidity and temperature sensor, using the i2c interface. |
| **apa102** | supported | - | - | This module provides Lua access to [APA102 RGB LEDs](https://youtu.be/UYvC-hukz-0) which are similar in function to the common [WS2812](ws2812) addressable LEDs. |
| **bit** | supported | supported | supported | Bit manipulation support, on 32bit integers. |
| **bme280** | supported | - | - | This module provides a simple interface to [BME280/BMP280 temperature/air presssure/humidity sensors](http://www.bosch-sensortec.com/bst/products/all_products/bme280) (Bosch Sensortec). |
| **bmp085** | supported | - | - | This module provides access to the [BMP085](https://www.sparkfun.com/tutorials/253) temperature and pressure sensor. |
| **cjson** | supported | - | - | This module has been replaced by [sjson](sjson.md). |
| **coap** | supported | - | - | The CoAP module provides a simple implementation according to [CoAP](http://tools.ietf.org/html/rfc7252) protocol. |
| **cron** | supported | - | - | [Cron](https://en.wikipedia.org/wiki/Cron)-like scheduler module. |
| **crypto** | supported | - | - | The crypto modules provides various functions for working with cryptographic algorithms. |
| **dht** | supported | supported | - | 
| **ds18b20** | supported | - | - | This module provides access to the DS18B20 1-Wire digital thermometer. |
| **encoder** | supported | - | - | The encoder modules provides various functions for encoding and decoding byte data. |
| **enduser-setup** | supported | - | - | This module provides a simple way of configuring ESP8266 chips without using a serial interface or pre-programming WiFi credentials onto the chip. |
| **[file](en/modules/file.md)** | supported | supported | supported | The file module provides access to the file system and its individual files. |
| **gdbstub** | supported | - | - | This module provides basic source code debugging of the firmware when used in conjunction with a version of gdb built for the lx106. |
| **[gpio](en/modules/gpio.md)** | supported | supported | supported | This module provides access to the [GPIO](https://en.wikipedia.org/wiki/General-purpose_input/output) (General Purpose Input/Output) subsystem. |
| **hdc1080** | supported | - | - | This module provides access to the [HDC1080](http://www.ti.com/product/HDC1080) low power, high accuracy digital humidity sensor with temperature sensor. |
| **hmc5883l** | supported | - | - | This module provides access to the [HMC5883L](https://www.sparkfun.com/products/10530) three axis digital compass. |
| **http** | supported | - | - | Basic HTTP *client* module that provides an interface to do GET/POST/PUT/DELETE over HTTP(S), as well as customized requests. |
| **hx711** | supported | - | - | This module provides access to an [HX711 load cell amplifier/ADC](https://learn.sparkfun.com/tutorials/load-cell-amplifier-hx711-breakout-hookup-guide). |
| **i2c** | supported | supported | - | 
| **l3g4200d** | supported | - | - | This module provides access to the [L3G4200D](https://www.sparkfun.com/products/10612) three axis digital gyroscope. |
| **mcp4725** | supported | - | - | This module provides access to the [MCP4725 12-bit Digital to Analog Converter](http://ww1.microchip.com/downloads/en/DeviceDoc/22039d.pdf). |
| **mdns** | supported | - | - | [Multicast DNS](https://en.wikipedia.org/wiki/Multicast_DNS) is used as part of Bonjour / Zeroconf. |
| **mqtt** | supported | - | - | The client adheres to version 3.1.1 of the [MQTT](https://en.wikipedia.org/wiki/MQTT) protocol. |
| **[net](en/modules/net.md)** | supported | supported | supported |  TLS operations was moved to the [TLS](tls.md) module  |
| **node** | supported | supported | supported | The node module provides access to system-level features such as sleep, restart and various info and IDs. |
| **ow** | supported | supported | - | This module provides functions to work with the [1-Wire](https://en.wikipedia.org/wiki/1-Wire) device communications bus system. |
| **pcm** | supported | - | - | Play sounds through various back-ends. |
| **perf** | supported | - | - | This module provides simple performance measurement for an application. |
| **pwm** | supported | - | - | 
| **rc** | supported | - | - | 
| **rfswitch** | supported | - | - | Module to operate 433/315Mhz devices like power outlet sockets, relays, etc. |
| **rotary** | supported | - | - | This module can read the state of cheap rotary encoder switches. |
| **rtcfifo** | supported | - | - | The rtcfifo module implements a first-in,first-out storage intended for sensor readings. |
| **rtcmem** | supported | - | - | The rtcmem module provides basic access to the [RTC](https://en.wikipedia.org/wiki/Real-time_clock) (Real Time Clock) memory. |
| **rtctime** | supported | - | - | The rtctime module provides advanced timekeeping support for NodeMCU, including keeping time across deep sleep cycles (provided [`rtctime.dsleep()`](#rtctimedsleep) is used instead of [`node.dsleep()`](node.md#nodedsleep)). |
| **si7021** | supported | - | - | This module provides access to the Si7021 humidity and temperature sensor. |
| **sigma-delta** | supported | supported | - | This module provides access to the [sigma-delta](https://en.wikipedia.org/wiki/Delta-sigma_modulation) component. |
| **sjson** | supported | - | supported | The JSON support module. |
| **sntp** | supported | - | - | The SNTP module implements a [Simple Network Time Procotol](https://en.wikipedia.org/wiki/Network_Time_Protocol#SNTP) client. |
| **somfy** | supported | - | - | This module provides a simple interface to control Somfy blinds via an RF transmitter (433.42 MHz). |
| **spi** | supported | supported | - | All transactions for sending and receiving are most-significant-bit first and least-significant last. |
| **struct** | supported | supported | - | This module offers basic facilities to convert Lua values to and from C structs. |
| **switec** | supported | - | - | This module controls a [Switec X.27](http://www.jukenswisstech.com/?page_id=103) (or compatible) instrument stepper motor. |
| **tcs34725** | supported | - | - | This module provides a simple interface to [TCS34725 colour/light sensors](https://www.adafruit.com/product/1334) (Adafruit). |
| **tls** | supported | - | - | SSL/TLS support |
| **tm1829** | supported | - | - | tm1829 is a library to handle led strips using Titan Micro tm1829 |
| **tmr** | supported | supported | supported | The tmr module allows access to simple timers, the system counter and uptime. |
| **tsl2561** | supported | - | - | 
| **u8g** | supported | - | - | U8glib is a graphics library developed at [olikraus/u8glib](https://github.com/olikraus/u8glib) with support for many different displays. |
| **uart** | supported | supported | - | The [UART](https://en.wikipedia.org/wiki/Universal_asynchronous_receiver/transmitter) (Universal asynchronous receiver/transmitter) module allows configuration of and communication over the UART serial port. |
| **ucg** | supported | - | - | Ucglib is a graphics library developed at [olikraus/ucglib](https://github.com/olikraus/ucglib) with support for color TFT displays. |
| **websocket** | supported | - | - | A websocket *client* module that implements [RFC6455](https://tools.ietf.org/html/rfc6455) (version 13) and provides a simple interface to send and receive messages. |
| **wifi** | supported | supported | - | 	The WiFi subsystem is maintained by background tasks that must run periodically. |
| **wps** | supported | - | - | [WPS](https://en.wikipedia.org/wiki/Wi-Fi_Protected_Setup) allows devices to be added to an existing network without entering the network credentials. |
| **ws2801** | supported | - | - | 
| **ws2812** | supported | supported | - | ws2812 is a library to handle ws2812-like led strips. |
| **xpt2046** | supported | - | - | XPT2046 is a touch controller used by several cheap displays - often in combination with the ILI9341 display controller. |
