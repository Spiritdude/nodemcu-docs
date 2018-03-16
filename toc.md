# NodeMCU API
| Module | esp8266 | esp32 | linux | Description |
| --- | --- | --- | --- | -- |
| adc | supported | supported | - | The ADC module provides access to the in-built ADC. |
| ads1115 | supported | - | - | This module provides access to the ADS1115 16-Bit analog-to-digital converter. |
| adxl345 | supported | - | - | 
| am2320 | supported | - | - | 
| apa102 | supported | - | - | This module provides Lua access to [APA102 RGB LEDs](https://youtu.be/UYvC-hukz-0) which are similar in function to the common [WS2812](ws2812) addressable LEDs. |
| bit | supported | supported | supported | 
| bme280 | supported | - | - | This module provides a simple interface to [BME280/BMP280 temperature/air presssure/humidity sensors](http://www.bosch-sensortec.com/bst/products/all_products/bme280) (Bosch Sensortec). |
| bmp085 | supported | - | - | 
| cjson | supported | - | - | This module has been replaced by [sjson](sjson.md). It provides a superset of functionality. All references to `cjson` can be replaced by `sjson`. |
| coap | supported | - | - | The CoAP module provides a simple implementation according to [CoAP](http://tools.ietf.org/html/rfc7252) protocol. |
| cron | supported | - | - | [Cron](https://en.wikipedia.org/wiki/Cron)-like scheduler module. |
| crypto | supported | - | - | The crypto modules provides various functions for working with cryptographic algorithms. |
| dht | supported | supported | - | 
| ds18b20 | supported | - | - | This module provides access to the DS18B20 1-Wire digital thermometer. Note that NodeMCU offers both a C module (this one) and [a Lua module for this sensor](https://github.com/nodemcu/nodemcu-firmware/tree/dev/lua_modules/ds18b20). See [#2003](https://github.com/nodemcu/nodemcu-firmware/pull/2003) for a discussion on the respective merits of them. |
| encoder | supported | - | - | The encoder modules provides various functions for encoding and decoding byte data. |
| enduser-setup | supported | - | - | This module provides a simple way of configuring ESP8266 chips without using a serial interface or pre-programming WiFi credentials onto the chip. |
| **[file](handbook/en/modules/file.md)** | supported | supported | supported | The file module provides access to the file system and its individual files. |
| gdbstub | supported | - | - | This module provides basic source code debugging of the firmware when used in conjunction with a version of gdb built for the lx106. If you enable this module, then fatal errors (like invalid memory reads) will trap into the gdbstub. This uses UART0 to talk to GDB. If this happens while the UART0 is connected to a terminal (or some IDE like esplorer) then you will see a string starting with `$T` and a few more characters after that. This is the signal that a trap has happened, and control should be passed to gdb. |
| **[gpio](handbook/en/modules/gpio.md)** | supported | supported | supported | 
| hdc1080 | supported | - | - | 
| hmc5883l | supported | - | - | 
| http | supported | - | - | Basic HTTP *client* module that provides an interface to do GET/POST/PUT/DELETE over HTTP(S), as well as customized requests. Due to the memory constraints on ESP8266, the supported page/body size is limited by available memory. Attempting to receive pages larger than this will fail. If larger page/body sizes are necessary, consider using [`net.createConnection()`](net.md#netcreateconnection) and stream in the data. |
| hx711 | supported | - | - | This module provides access to an [HX711 load cell amplifier/ADC](https://learn.sparkfun.com/tutorials/load-cell-amplifier-hx711-breakout-hookup-guide). The HX711 is an inexpensive 24bit ADC with programmable 128x, 64x, and 32x gain. Currently only channel A at 128x gain is supported. |
| i2c | supported | supported | - | 
| l3g4200d | supported | - | - | 
| mcp4725 | supported | - | - | 
| mdns | supported | - | - | [Multicast DNS](https://en.wikipedia.org/wiki/Multicast_DNS) is used as part of Bonjour / Zeroconf. This allows system to identify themselves and the services that they provide on a local area network. Clients are then able to discover these systems and connect to them.  |
| mqtt | supported | - | - | 
| net | supported | supported | supported | ** TLS operations was moved to the [TLS](tls.md) module ** |
| node | supported | supported | supported | The node module provides access to system-level features such as sleep, restart and various info and IDs. |
| ow | supported | supported | - | This module provides functions to work with the [1-Wire](https://en.wikipedia.org/wiki/1-Wire) device communications bus system. |
| pcm | supported | - | - | Play sounds through various back-ends. |
| perf | supported | - | - | 
| pwm | supported | - | - | 
| rc | supported | - | - | 
| rfswitch | supported | - | - | 
| rotary | supported | - | - | 
| rtcfifo | supported | - | - | The rtcfifo module implements a first-in,first-out storage intended for sensor readings. As the name suggests, it is backed by the [RTC](https://en.wikipedia.org/wiki/Real-time_clock) user memory and as such survives deep sleep cycles. Conceptually it can be thought of as a cyclic array of `{ timestamp, name, value }` tuples. Internally it uses a space-optimized storage format to allow the greatest number of samples to be kept. This comes with several trade-offs, and as such is not a one-solution-fits-all. Notably: |
| rtcmem | supported | - | - | The rtcmem module provides basic access to the [RTC](https://en.wikipedia.org/wiki/Real-time_clock) (Real Time Clock) memory. |
| rtctime | supported | - | - | The rtctime module provides advanced timekeeping support for NodeMCU, including keeping time across deep sleep cycles (provided [`rtctime.dsleep()`](#rtctimedsleep) is used instead of [`node.dsleep()`](node.md#nodedsleep)). This can be used to significantly extend battery life on battery powered sensor nodes, as it is no longer necessary to fire up the RF module each wake-up in order to obtain an accurate timestamp. |
| si7021 | supported | - | - | This module provides access to the Si7021 humidity and temperature sensor. |
| sigma-delta | supported | supported | - | This module provides access to the [sigma-delta](https://en.wikipedia.org/wiki/Delta-sigma_modulation) component. It's a hardware signal generator that can be routed to any of the GPIOs except pin 0. |
| sjson | supported | - | supported | The JSON support module. Allows encoding and decoding to/from JSON. |
| sntp | supported | - | - | The SNTP module implements a [Simple Network Time Procotol](https://en.wikipedia.org/wiki/Network_Time_Protocol#SNTP) client. This includes support for the "anycast" [NTP](https://en.wikipedia.org/wiki/Network_Time_Protocol) mode where, if supported by the NTP server(s) in your network, it is not necessary to even know the IP address of the NTP server. |
| somfy | supported | - | - | This module provides a simple interface to control Somfy blinds via an RF transmitter (433.42 MHz). It is based on [Nickduino Somfy Remote Arduino skecth](https://github.com/Nickduino/Somfy_Remote).  |
| spi | supported | supported | - | All transactions for sending and receiving are most-significant-bit first and least-significant last. |
| struct | supported | supported | - | This module offers basic facilities to convert Lua values to and from C structs. Its main functions are `struct.pack`, which packs multiple Lua values into a struct-like string; and `struct.unpack`, which unpacks multiple Lua values from a given struct-like string. |
| switec | supported | - | - | This module controls a [Switec X.27](http://www.jukenswisstech.com/?page_id=103) (or compatible) instrument stepper motor. These are the  |
| tcs34725 | supported | - | - | This module provides a simple interface to [TCS34725 colour/light sensors](https://www.adafruit.com/product/1334) (Adafruit). |
| tls | supported | - | - | **SSL/TLS support** |
| tm1829 | supported | - | - | tm1829 is a library to handle led strips using Titan Micro tm1829 |
| tmr | supported | supported | supported | The tmr module allows access to simple timers, the system counter and uptime. |
| tsl2561 | supported | - | - | 
| u8g | supported | - | - | U8glib is a graphics library developed at [olikraus/u8glib](https://github.com/olikraus/u8glib) with support for many different displays. The NodeMCU firmware supports a subset of these. |
| uart | supported | supported | - | The [UART](https://en.wikipedia.org/wiki/Universal_asynchronous_receiver/transmitter) (Universal asynchronous receiver/transmitter) module allows configuration of and communication over the UART serial port. |
| ucg | supported | - | - | Ucglib is a graphics library developed at [olikraus/ucglib](https://github.com/olikraus/ucglib) with support for color TFT displays. The NodeMCU firmware supports a subset of these: |
| websocket | supported | - | - | A websocket *client* module that implements [RFC6455](https://tools.ietf.org/html/rfc6455) (version 13) and provides a simple interface to send and receive messages. |
| wifi | supported | supported | - | !!! important |
| wps | supported | - | - | [WPS](https://en.wikipedia.org/wiki/Wi-Fi_Protected_Setup) allows devices to be added to an existing network without entering the network credentials. |
| ws2801 | supported | - | - | 
| ws2812 | supported | supported | - | ws2812 is a library to handle ws2812-like led strips. |
| xpt2046 | supported | - | - | XPT2046 is a touch controller used by several cheap displays - often in combination with the ILI9341 display controller. |
