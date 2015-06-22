# Web of Things Framework for ESP8266

This will be an experimental implementation of the Web of Things Framework written in the C programming language for the ESP8266. This project is a sister of the [NodeJS server for the Web of Things](https://github.com/w3c/web-of-things-framework) and the [Arduino server for the Web of Things](https://github.com/w3c/arduino-wot).

A hundred billion IoT devices are expected to be deployed over the next ten years. There are many IoT platforms, and an increasing number of IoT technologies. However, the IoT products are currently beset by silos and a lack of interoperability, which blocks the benefits of the network effect from taking hold.  At W3C, we are exploring the potential for bridging IoT platforms and devices through the World Wide Web via a new class of Web servers that are connected through a common framework, and available in a variety of scales from microcontrollers, to smart phones and home/office hubs, and cloud-based server farms.

This framework involves virtual objects ("things") as proxies for physical and abstract entities. These things are modelled in terms of metadata, events, properties and actions, with bindings to scripting APIs and a variety of protocols, since no one protocol will fulfil all needs. This server will start with bindings to MQTT and CoAP, and may later add bindings for HTTP and WebSockets.

## Technical Details

The ESP8266 is a 32 bit microcontroller with an integrated WiFi transceiver and support for TCP/IP. It is based on the Harvard architecture, and has split instruction and data paths. The MCU has 64KB instruction RAM, 96 KB data RAM, and 64KB Boot ROM. There are a family of boards, the most common of which are the ESP-01 and the ESP-12. The ESP-01 offers 512KB FLASH memory compared to 4MB for the ESP-12.  The latter breaks out more of the ESP8266 pins and is generally a better choice for projects. Both the ESP-01 and ESP-12 include an antenna on the PCB. There are multiple GPIO pins, one 10-bit ADC for analog input, and support for PWM for analog output. There is a UART and support for SPI and I2C based interfaces.

* [Arduino-compatible IDE with ESP8266 support](https://github.com/esp8266/Arduino) - makes it easy to re-use existing code and libraries for the Arduino.
* [NodeMCU](http://nodemcu.com/index_en.html) - firmware that integrates the Lua scripting language with a comprehensive library including support for SPI, I2C, HTTP, MQTT and CoAP.
* [MicroPython](https://github.com/micropython/micropython/tree/master/esp8266) - a experimental implementation of the micro-python interpreter for the ESP8266.

This project will explore C-based implementations of the Web of Things Framework, as well as Lua-based implementations using NodeMCU.

## Prerequisites

 *to be deterimined when we have some code that can be built and run*
  
## Installation

The starting point is to install Git, see:

  http://git-scm.com/book/en/v2/Getting-Started-Installing-Git

Next create a copy of this directory and change to it as follows:

```
  git clone https://github.com/w3c/wot-esp8266
  cd wot-esp8266
```

## Contributing

[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/w3c/web-of-things-framework?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

We welcome contributions. If you find a bug in the source code or a mistake in the documentation, you can help us by submitting an issue to our [GitHub repository](https://github.com/w3c/arduino-wot), and likewise if you have suggestions for new features. Even better you can submit a Pull Request with a fix. We also have a Gitter chat channel, see above link.

We encourage you to join the W3C [Web of Things Community Group](https://www.w3.org/community/wot/) where contribution and discussions happen. Anyone can join and there are no fees.

The amount of time you contribute and the areas in which you contribute is up to you. 

## License

(The MIT License)

Copyright (c) 2015 Dave Raggett &lt;dsr@w3.org&gt;

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
