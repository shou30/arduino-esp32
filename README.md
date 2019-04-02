# Arduino core for ESP32 WiFi chip    [![Build Status](https://travis-ci.org/espressif/arduino-esp32.svg?branch=master)](https://travis-ci.org/espressif/arduino-esp32)

### Need help or have a question? Join the chat at [![https://gitter.im/espressif/arduino-esp32](https://badges.gitter.im/espressif/arduino-esp32.svg)](https://gitter.im/espressif/arduino-esp32?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

## Contents
- [Development Status](#development-status)
- [Installation Instructions](#installation-instructions)
- [Decoding Exceptions](#decoding-exceptions)
- [Issue/Bug report template](#issuebug-report-template)
- [ESP32Dev Board PINMAP](#esp32dev-board-pinmap)

## Development Status
[Latest stable release ![Release Version](https://img.shields.io/github/release/espressif/arduino-esp32.svg?style=plastic) ![Release Date](https://img.shields.io/github/release-date/espressif/arduino-esp32.svg?style=plastic)](https://github.com/espressif/arduino-esp32/releases/latest/) ![Downloads](https://img.shields.io/github/downloads/espressif/arduino-esp32/latest/total.svg?style=plastic)

[Latest development release ![Development Version](https://img.shields.io/github/release/espressif/arduino-esp32/all.svg?style=plastic) ![Development Date](https://img.shields.io/github/release-date-pre/espressif/arduino-esp32.svg?style=plastic)](https://github.com/espressif/arduino-esp32/releases/latest/) ![Downloads](https://img.shields.io/github/downloads-pre/espressif/arduino-esp32/latest/total.svg?style=plastic)

Most of the framework is implemented. Most noticable is the missing analogWrite. While analogWrite is on it's way, there are a few other options that you can use:
- 16 channels [LEDC](cores/esp32/esp32-hal-ledc.h) which is PWM
- 8 channels [SigmaDelta](cores/esp32/esp32-hal-sigmadelta.h) which uses SigmaDelta modulation
- 2 channels [DAC](cores/esp32/esp32-hal-dac.h) which gives real analog output

## Installation Instructions
- Using Arduino IDE Boards Manager (preferred)
  + [Instructions for Boards Manager](docs/arduino-ide/boards_manager.md)
- Using Arduino IDE with the development repository
  + [Instructions for Windows](docs/arduino-ide/windows.md)
  + [Instructions for Mac](docs/arduino-ide/mac.md)
  + [Instructions for Debian/Ubuntu Linux](docs/arduino-ide/debian_ubuntu.md)
  + [Instructions for Fedora](docs/arduino-ide/fedora.md)
  + [Instructions for openSUSE](docs/arduino-ide/opensuse.md)
- [Using PlatformIO](docs/platformio.md)
- [Building with make](docs/make.md)
- [Using as ESP-IDF component](docs/esp-idf_component.md)
- [Using OTAWebUpdater](docs/OTAWebUpdate/OTAWebUpdate.md)

#### Decoding exceptions

You can use [EspExceptionDecoder](https://github.com/me-no-dev/EspExceptionDecoder) to get meaningful call trace.

#### Issue/Bug report template
Before reporting an issue, make sure you've searched for similar one that was already created. Also make sure to go through all the issues labelled as [for reference](https://github.com/espressif/arduino-esp32/issues?utf8=%E2%9C%93&q=is%3Aissue%20label%3A%22for%20reference%22%20).

Finally, if you're sure no one else had the issue, follow the [ISSUE_TEMPLATE](docs/ISSUE_TEMPLATE.md) while reporting any issue.

You must check out [LCSC](https://lcsc.com/) for ordering good quality components for good prices.

There is no minimum quantity order that you need to purchase for getting it shipped. [LCSC](https://lcsc.com/) is the leading chinese electronics parts supplier. You can find all the conponents for your project from smd parts to through hole parts and even development boards, sensors etc and that too for very good pricing. You will also get a discount on your first order.

![alt text](https://github.com/akarsh98/ESP8266-Ra-02-arduino-code/blob/master/SCREENSHOTS/lcsc.JPG?raw=true)

You must check out [JLCPCB](https://jlcpcb.com/m) for ordering PCBs online for cheap!

You get 10 good quality PCBs manufactured and shipped to your doorstep for 2$ and some shipping. You will also get a discount on shipping on your first order. To design your own PCB head over to [easyEDA](https://easyeda.com/), once that is done upload your Gerber files onto [JLCPCB](https://jlcpcb.com/m) to get them manufactured with good quality and quick turnaround time.

![alt text](https://github.com/akarsh98/DFRobot-LoRa-Firebeetle-Code/blob/master/SCREENSHOTS/JLCFULL.jpg?raw=true)

## ESP32Dev Board PINMAP

![Pin Functions](docs/esp32_pinmap.png)

## Hint

Sometimes to program ESP32 via serial you must keep GPIO0 LOW during the programming process
