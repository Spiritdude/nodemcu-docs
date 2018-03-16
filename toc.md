# NodeMCU API
| Module | esp8266 | esp32 | linux | Description |
| --- | --- | --- | --- | -- |
| adc | supported | supported | - | <sub><sup>The ADC module provides access to the in-built ADC.</sup></sub> |
| ads1115 | supported | - | - | <sub><sup>This module provides access to the ADS1115 16-Bit analog-to-digital converter.</sup></sub> |
| adxl345 | supported | - | - | <sub><sup>This module provides access to the [ADXL345](https://www.sparkfun.com/products/9836) triple axis accelerometer.</sup></sub> |
| am2320 | supported | - | - | <sub><sup>This module provides access to the [AM2320](https://akizukidenshi.com/download/ds/aosong/AM2320.pdf) humidity and temperature sensor, using the i2c interface.</sup></sub> |
| apa102 | supported | - | - | <sub><sup>This module provides Lua access to [APA102 RGB LEDs](https://youtu.be/UYvC-hukz-0) which are similar in function to the common [WS2812](ws2812) addressable LEDs.</sup></sub> |
| bit | supported | supported | supported | <sub><sup>Bit manipulation support, on 32bit integers.</sup></sub> |
| bme280 | supported | - | - | <sub><sup>This module provides a simple interface to [BME280/BMP280 temperature/air presssure/humidity sensors](http://www.bosch-sensortec.com/bst/products/all_products/bme280) (Bosch Sensortec).</sup></sub> |
| bmp085 | supported | - | - | <sub><sup>This module provides access to the [BMP085](https://www.sparkfun.com/tutorials/253) temperature and pressure sensor. The module also works with BMP180.</sup></sub> |
| cjson | supported | - | - | <sub><sup>This module has been replaced by [sjson](sjson.md). It provides a superset of functionality. All references to `cjson` can be replaced by `sjson`.</sup></sub> |
| coap | supported | - | - | <sub><sup>The CoAP module provides a simple implementation according to [CoAP](http://tools.ietf.org/html/rfc7252) protocol.</sup></sub> |
| cron | supported | - | - | <sub><sup>[Cron](https://en.wikipedia.org/wiki/Cron)-like scheduler module.</sup></sub> |
| crypto | supported | - | - | <sub><sup>The crypto modules provides various functions for working with cryptographic algorithms.</sup></sub> |
| dht | supported | supported | - | 
| ds18b20 | supported | - | - | <sub><sup>This module provides access to the DS18B20 1-Wire digital thermometer. Note that NodeMCU offers both a C module (this one) and [a Lua module for this sensor](https://github.com/nodemcu/nodemcu-firmware/tree/dev/lua_modules/ds18b20). See [#2003](https://github.com/nodemcu/nodemcu-firmware/pull/2003) for a discussion on the respective merits of them.</sup></sub> |
| encoder | supported | - | - | <sub><sup>The encoder modules provides various functions for encoding and decoding byte data.</sup></sub> |
| enduser-setup | supported | - | - | <sub><sup>This module provides a simple way of configuring ESP8266 chips without using a serial interface or pre-programming WiFi credentials onto the chip.</sup></sub> |
| **[file](handbook/en/modules/file.md)** | supported | supported | supported | <sub><sup>The file module provides access to the file system and its individual files.</sup></sub> |
| gdbstub | supported | - | - | <sub><sup>This module provides basic source code debugging of the firmware when used in conjunction with a version of gdb built for the lx106. If you enable this module, then fatal errors (like invalid memory reads) will trap into the gdbstub. This uses UART0 to talk to GDB. If this happens while the UART0 is connected to a terminal (or some IDE like esplorer) then you will see a string starting with `$T` and a few more characters after that. This is the signal that a trap has happened, and control should be passed to gdb.</sup></sub> |
| **[gpio](handbook/en/modules/gpio.md)** | supported | supported | supported | <sub><sup>This module provides access to the [GPIO](https://en.wikipedia.org/wiki/General-purpose_input/output) (General Purpose Input/Output) subsystem.</sup></sub> |
| hdc1080 | supported | - | - | <sub><sup>This module provides access to the [HDC1080](http://www.ti.com/product/HDC1080) low power, high accuracy digital humidity sensor with temperature sensor.</sup></sub> |
| hmc5883l | supported | - | - | <sub><sup>This module provides access to the [HMC5883L](https://www.sparkfun.com/products/10530) three axis digital compass.</sup></sub> |
| http | supported | - | - | <sub><sup>Basic HTTP *client* module that provides an interface to do GET/POST/PUT/DELETE over HTTP(S), as well as customized requests. Due to the memory constraints on ESP8266, the supported page/body size is limited by available memory. Attempting to receive pages larger than this will fail. If larger page/body sizes are necessary, consider using [`net.createConnection()`](net.md#netcreateconnection) and stream in the data.</sup></sub> |
| hx711 | supported | - | - | <sub><sup>This module provides access to an [HX711 load cell amplifier/ADC](https://learn.sparkfun.com/tutorials/load-cell-amplifier-hx711-breakout-hookup-guide). The HX711 is an inexpensive 24bit ADC with programmable 128x, 64x, and 32x gain. Currently only channel A at 128x gain is supported.</sup></sub> |
| i2c | supported | supported | - | 
| l3g4200d | supported | - | - | <sub><sup>This module provides access to the [L3G4200D](https://www.sparkfun.com/products/10612) three axis digital gyroscope.</sup></sub> |
| mcp4725 | supported | - | - | <sub><sup>This module provides access to the [MCP4725 12-bit Digital to Analog Converter](http://ww1.microchip.com/downloads/en/DeviceDoc/22039d.pdf).</sup></sub> |
| mdns | supported | - | - | <sub><sup>[Multicast DNS](https://en.wikipedia.org/wiki/Multicast_DNS) is used as part of Bonjour / Zeroconf. This allows system to identify themselves and the services that they provide on a local area network. Clients are then able to discover these systems and connect to them. </sup></sub> |
| mqtt | supported | - | - | <sub><sup>The client adheres to version 3.1.1 of the [MQTT](https://en.wikipedia.org/wiki/MQTT) protocol. Make sure that your broker supports and is correctly configured for version 3.1.1. The client is backwards incompatible with brokers running MQTT 3.1.</sup></sub> |
| net | supported | supported | supported | <sub><sup>** TLS operations was moved to the [TLS](tls.md) module **</sup></sub> |
| node | supported | supported | supported | <sub><sup>The node module provides access to system-level features such as sleep, restart and various info and IDs.</sup></sub> |
| ow | supported | supported | - | <sub><sup>This module provides functions to work with the [1-Wire](https://en.wikipedia.org/wiki/1-Wire) device communications bus system.</sup></sub> |
| pcm | supported | - | - | <sub><sup>Play sounds through various back-ends.</sup></sub> |
| perf | supported | - | - | <sub><sup>This module provides simple performance measurement for an application. It samples the program counter roughly every 50 microseconds and builds a histogram of the values that it finds. Since there is only a small amount</sup></sub> |
| pwm | supported | - | - | 
| rc | supported | - | - | 
| rfswitch | supported | - | - | <sub><sup>Module to operate 433/315Mhz devices like power outlet sockets, relays, etc. This will most likely work with all popular low cost power outlet sockets with a SC5262 / SC5272, HX2262 / HX2272, PT2262 / PT2272, EV1527, RT1527, FP1527 or HS1527 chipset.</sup></sub> |
| rotary | supported | - | - | <sub><sup>This module can read the state of cheap rotary encoder switches. These are available at all the standard places for a dollar or two. They are five pin devices where three are used for a gray code encoder for rotation, and two are used for the push switch. These switches are commonly used in car audio systems. </sup></sub> |
| rtcfifo | supported | - | - | <sub><sup>The rtcfifo module implements a first-in,first-out storage intended for sensor readings. As the name suggests, it is backed by the [RTC](https://en.wikipedia.org/wiki/Real-time_clock) user memory and as such survives deep sleep cycles. Conceptually it can be thought of as a cyclic array of `{ timestamp, name, value }` tuples. Internally it uses a space-optimized storage format to allow the greatest number of samples to be kept. This comes with several trade-offs, and as such is not a one-solution-fits-all. Notably:</sup></sub> |
| rtcmem | supported | - | - | <sub><sup>The rtcmem module provides basic access to the [RTC](https://en.wikipedia.org/wiki/Real-time_clock) (Real Time Clock) memory.</sup></sub> |
| rtctime | supported | - | - | <sub><sup>The rtctime module provides advanced timekeeping support for NodeMCU, including keeping time across deep sleep cycles (provided [`rtctime.dsleep()`](#rtctimedsleep) is used instead of [`node.dsleep()`](node.md#nodedsleep)). This can be used to significantly extend battery life on battery powered sensor nodes, as it is no longer necessary to fire up the RF module each wake-up in order to obtain an accurate timestamp.</sup></sub> |
| si7021 | supported | - | - | <sub><sup>This module provides access to the Si7021 humidity and temperature sensor.</sup></sub> |
| sigma-delta | supported | supported | - | <sub><sup>This module provides access to the [sigma-delta](https://en.wikipedia.org/wiki/Delta-sigma_modulation) component. It's a hardware signal generator that can be routed to any of the GPIOs except pin 0.</sup></sub> |
| sjson | supported | - | supported | <sub><sup>The JSON support module. Allows encoding and decoding to/from JSON.</sup></sub> |
| sntp | supported | - | - | <sub><sup>The SNTP module implements a [Simple Network Time Procotol](https://en.wikipedia.org/wiki/Network_Time_Protocol#SNTP) client. This includes support for the "anycast" [NTP](https://en.wikipedia.org/wiki/Network_Time_Protocol) mode where, if supported by the NTP server(s) in your network, it is not necessary to even know the IP address of the NTP server.</sup></sub> |
| somfy | supported | - | - | <sub><sup>This module provides a simple interface to control Somfy blinds via an RF transmitter (433.42 MHz). It is based on [Nickduino Somfy Remote Arduino skecth](https://github.com/Nickduino/Somfy_Remote). </sup></sub> |
| spi | supported | supported | - | <sub><sup>All transactions for sending and receiving are most-significant-bit first and least-significant last.</sup></sub> |
| struct | supported | supported | - | <sub><sup>This module offers basic facilities to convert Lua values to and from C structs. Its main functions are `struct.pack`, which packs multiple Lua values into a struct-like string; and `struct.unpack`, which unpacks multiple Lua values from a given struct-like string.</sup></sub> |
| switec | supported | - | - | <sub><sup>This module controls a [Switec X.27](http://www.jukenswisstech.com/?page_id=103) (or compatible) instrument stepper motor. These are the </sup></sub> |
| tcs34725 | supported | - | - | <sub><sup>This module provides a simple interface to [TCS34725 colour/light sensors](https://www.adafruit.com/product/1334) (Adafruit).</sup></sub> |
| tls | supported | - | - | <sub><sup>**SSL/TLS support**</sup></sub> |
| tm1829 | supported | - | - | <sub><sup>tm1829 is a library to handle led strips using Titan Micro tm1829</sup></sub> |
| tmr | supported | supported | supported | <sub><sup>The tmr module allows access to simple timers, the system counter and uptime.</sup></sub> |
| tsl2561 | supported | - | - | 
| u8g | supported | - | - | <sub><sup>U8glib is a graphics library developed at [olikraus/u8glib](https://github.com/olikraus/u8glib) with support for many different displays. The NodeMCU firmware supports a subset of these.</sup></sub> |
| uart | supported | supported | - | <sub><sup>The [UART](https://en.wikipedia.org/wiki/Universal_asynchronous_receiver/transmitter) (Universal asynchronous receiver/transmitter) module allows configuration of and communication over the UART serial port.</sup></sub> |
| ucg | supported | - | - | <sub><sup>Ucglib is a graphics library developed at [olikraus/ucglib](https://github.com/olikraus/ucglib) with support for color TFT displays. The NodeMCU firmware supports a subset of these:</sup></sub> |
| websocket | supported | - | - | <sub><sup>A websocket *client* module that implements [RFC6455](https://tools.ietf.org/html/rfc6455) (version 13) and provides a simple interface to send and receive messages.</sup></sub> |
| wifi | supported | supported | - | <sub><sup>!!! important</sup></sub> |
| wps | supported | - | - | <sub><sup>[WPS](https://en.wikipedia.org/wiki/Wi-Fi_Protected_Setup) allows devices to be added to an existing network without entering the network credentials.</sup></sub> |
| ws2801 | supported | - | - | 
| ws2812 | supported | supported | - | <sub><sup>ws2812 is a library to handle ws2812-like led strips.</sup></sub> |
| xpt2046 | supported | - | - | <sub><sup>XPT2046 is a touch controller used by several cheap displays - often in combination with the ILI9341 display controller.</sup></sub> |
