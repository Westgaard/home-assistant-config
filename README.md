# home-assistant-config

Config-files and settings for my Home Assistant and smarthome. So that I easily can set it up if I break my SD-card (Again). Or drown my Rpi (Again). Or fry my Hue-hub (Again). 

## Hardware
- Raspberry Pi 4
- 5.1V 3A power adapter (Important to use a proper power adapter!) 
- Slide case (Be careful not to break your SD-card when sliding it together...) 
- Sonoff Zigbee 3.0 USB dongle
- 20 cm USB-extender for Sonoff
- Philips Hue hub
- Futurehome hub V1.0 (Zwave/enocean)
- USB to SATA
- SSD Drive

## Installation of Home Assistant OS to SSD
1. Download and install Rasperry Pi imager: https://www.raspberrypi.com/software/
2. Run Pi Imager, select OS, Misc utility images, Bootloader, USB Boot. Select SD-card and Write
3. Put SD-card in RPi4, power up RPi, wait 30 seconds, remove power.
4. Connect USB to sata with SDD to computer, run Pi Imager again
5. Select OS, Other specific-purpose OS, Home assistants and home automation, Home Assistant, Home Assistant OS 9.4 (RPi 4/400), select SSD, Write.
6. Connect USB to sata to RPi USB 3.0-port, power up RPi.
7. Go grab a coffee, and the connect to homeassistant.local:8123 and restore backup.
