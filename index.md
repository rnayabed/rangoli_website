---
layout: default
---

## Disclaimer
**Rangoli is NOT official software. I am not affiliated to Royal Kludge and only maintain this software in my free time. There is no gurantee that it will work with your keyboard. I only own a single RK keyboard (RK71RGB N Wired) and pieced up it's protocol and assumed that all keyboards that I could find in the official software use the same protocol. There is no documentation available for RK Software protocol. If your keyboard does not work, please create a bug report. You can also check [Supported Keyboards](https://github.com/rnayabed/rangoli/blob/master/supported-keyboards.md) list.**

## Download

![version](https://img.shields.io/badge/Version-2.0-green)
![Total Downloads](https://img.shields.io/github/downloads/rnayabed/rangoli/total?label=Total%20Downloads)
[![Tip Me via PayPal](https://img.shields.io/badge/PayPal-Tip%20me-blue.svg?logo=paypal)](https://www.paypal.me/rnayabed)
[![Tip Me via Ko-Fi](https://img.shields.io/badge/Ko--Fi-Tip%20me-red.svg?logo=kofi)](https://ko-fi.com/rnayabed)

### Linux x86_64
**Note: You need to have libxcb-xinerama0 (for multi monitor support) and xterm (udev writer prompt) installed.**
- [Installer (.run)](https://github.com/rnayabed/rangoli/releases/download/2.0/rangoli-installer-linux-64.run)
- [Portable (.zip)](https://github.com/rnayabed/rangoli/releases/download/2.0/rangoli-portable-linux-64.zip)

### Windows x86_64
- [Installer (.exe)](https://github.com/rnayabed/rangoli/releases/download/2.0/rangoli-installer-windows-64.exe)
- [Portable (.zip)](https://github.com/rnayabed/rangoli/releases/download/2.0/rangoli-portable-windows-64.zip)

### MacOS
- [Installer (.app)](https://github.com/rnayabed/rangoli/releases/download/2.0/rangoli-installer-macos.app.zip)
- [Portable (.zip)](https://github.com/rnayabed/rangoli/releases/download/2.0/rangoli-portable-macos.zip)


# Changelog

* Auto update checker
* Add support for multiple VID but same protocol
* Update udev-writer script
* Fix MacOS
* Add multiple Col Support for Windows
* Add logging

[Full Changelog](https://github.com/rnayabed/rangoli/compare/1.0...2.0)

## Demonstration Video

<iframe width="640" height="360" src="https://www.youtube.com/embed/MTGICKC4G5U">
</iframe>
<br/>

## Screenshots

You can view screenshots over [here](./screenshots.html#screenshots).

## Purpose

[Royal Kludge Keyboards](https://rkgamingstore.com/) are very popular in the budget mechanical keyboard community. Sometimes it is the only viable option for students especially from developing countries like me. However, they are infamous for poor software support.

There are efforts to get 3rd party firmware like [QMK](https://qmk.fm/) to run on some of these keyboards, but not every keyboard is supported. Also there are keyboards with the same model name but different processors. The entire process is risky and not recommended for begineers.

I decided to try another approach to this problem. I reverse engineered the protocol these keyboards use with their default firmware. I did this by using [Wireshark](https://www.wireshark.org/) to capture and observe USB packets sent from my PC to my keyboard after editing settings in the RK Software.

Therefore, instead of changing the keyboard firmware, this software pretends to be "RK Software". There is no risk of bricking your keyboard. It is plug and play!

## Pros over RK Software
- Free and Open Source.
- Cross-platform. Rangoli runs on Linux, Windows and MacOS.
- Start On Boot. You can configure Rangoli to start at system boot and also select a profile to be applied on startup.
- Functional System Tray Icon. Although the RK Software does show up in System Tray, it is very limited and opens up the main window for even basic tasks like selecting a profile. Rangoli offers more functionality, including the ability to apply a profile per keyboard.
- Modern. Far more user friendly and has basic window behaviours including being able to resize, maximise, etc - something which the RK Software lacks.
- Colour Picker. You can select colour of your choice directly from your screen. Hex, RGB, HSV, HSL are also supported.
- Customisable. Rangoli offers users to change it's theme colours and also offers light and dark themes.

## Supported features
- Custom Key Map
- All built-in light modes
- Per key RGB
- Per key LED Brightness, Animation and Sleep

## Planned features
- Music Mode
- Custom RGB Patterns

## Features that will not be worked on
- Macros. This is something that can be done directly on OS level. There are tools like [AutoHotkey](https://www.autohotkey.com/) and [AutoKey](https://github.com/autokey/autokey) that does this far better than RK Software itself.
- Keyboard Firmware update. I was not able to reverse engineer this aspect of the RK Software because the function itself is broken.

## Supported Keyboards

Full list of supported keyboards can be found [here](https://github.com/rnayabed/rangoli/blob/master/supported-keyboards.md).

## Bugs and Support

If you want to report an issue or sugggest a feature, please report it by creating a [GitHub issue](https://github.com/rnayabed/rangoli/issues).

You may also contact me via any of the following platforms:
- E-Mail: [debayansutradhar3@gmail.com](mailto:debayansutradhar3@gmail.com)
- Matrix: @dubbadhar:matrix.org
- Discord: rnayabed#0784

## Donate

It takes a lot of time and effort to build quality software. Anything will be highly appreciated <3

- UPI: 9903299105@upi
- [Ko-Fi](https://ko-fi.com/rnayabed)
- [Paypal](https://paypal.me/rnayabed)

## License

Rangoli is licensed to [GNU General Public License v3.0](https://github.com/rnayabed/rangoli/blob/master/LICENSE).

```
Rangoli - Free, Open Source, Lightweight, Cross-platform Software for Royal Kludge Keyboards
Copyright (C) 2023 Debayan Sutradhar (rnayabed)

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.
This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.
```
