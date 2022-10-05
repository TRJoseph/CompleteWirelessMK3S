# Comprehensive Wireless Set-Up for the Prusa MK3/MK3S 3D Printer

Hello! This repository hosts multiple different mini projects/modifications all in one organized package in order to add wireless communication and monitoring to your Prusa MK3/S 3D Printer.

## PrusaLink/Prusa Connect
This software is provided by Prusa Research and aims to provide a wireless experience to your 3D Printer.

Link to guide:
https://help.prusa3d.com/guide/prusalink-and-prusa-connect-setup-for-mk3-s-_221744

Required Parts:
- Raspberry Pi Zero W/2W: https://a.co/d/hA2GZVA
- 16Gb/32Gb/64Gb SD Card: https://a.co/d/cL8JP7L
- Two .stl Files that provide shielding and mounting for the Pi: https://www.printables.com/model/36118-raspberry-pi-zero-frame-for-einsy-rambo#_ga=2.4796091.928477907.1663790514-1145385291.1662414219
- GPIo Pin Headers (18/19mm): https://a.co/d/74iuOg9
- PETG Filament: https://a.co/d/5tQsqOI


## ESP32 Live-Feed Camera
Another essential part of the wireless overhaul to this printer is a streaming camera so you are able to monitor your prints remotely. This can be accomplished with a cheap purchase of an ESP32 camera.

Required Parts for the build:
- ESP32: https://a.co/d/fkvw7ga
- Power Supply module to power the Camera: https://a.co/d/hhnKFhK

I have created a modified version of the Arduino core ESP32 firmware to include functionality using the onboard flashlight to help visuals in low-light situations. This code is available [here](https://github.com/TRJoseph/CompleteWirelessMK3S/tree/main/ESP32). 
![flashlight](/Docs/ReadMeImages/esp32flashlight.png)

If you wish to use the original code, inside of your Arduino IDE navigate to File > Examples > ESP32 > Camera > CameraWebServer

