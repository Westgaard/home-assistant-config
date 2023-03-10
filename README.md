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
3. Put SD-card in RPi4, power up RPi, wait 30 seconds, remove power, remove SD-card and throw it away
4. Connect USB to sata with SDD to computer, run Pi Imager again
5. Select OS, Other specific-purpose OS, Home assistants and home automation, Home Assistant, Home Assistant OS 9.4 (RPi 4/400), select SSD and Write.
6. Connect USB to sata to RPi USB 3.0-port, power up RPi.
7. Go grab a coffee, and the connect to homeassistant.local:8123 and restore backup.

## Add-ons
- [HACS](https://hacs.xyz/)
- [Auto Backup](https://github.com/jcwillox/hass-auto-backup) from HACS
- Samba share - Folder with backup-files from Auto backup mounted on computer which syncs to Jottacloud
- [Futurehome2mqtt](https://github.com/runelangseid/hassio-futurehome2mqtt) - Expose (some of) the devices in Futurehome to HA
  - Connected to Futurehome-hub
- [Zigbee2MQTT](https://www.zigbee2mqtt.io/)
  - Bridged to Futurehome, se [Mosquitto.conf](https://github.com/Westgaard/home-assistant-config/blob/main/share/mosquitto/mosquitto.conf)
- [Leaf2mqtt](https://github.com/yp87/leaf2mqtt) - To get battery-status from Nissan Leaf
- [Mosquitto broker](https://github.com/home-assistant/addons/tree/master/mosquitto)
  - Bridge to Futurehome, broker for Zigbee2MQTT

## Configuration
- [Configuration.yaml](https://github.com/Westgaard/home-assistant-config/blob/main/config/configuration.yaml)
- [Automations.yaml](https://github.com/Westgaard/home-assistant-config/blob/main/config/automations.yaml)
