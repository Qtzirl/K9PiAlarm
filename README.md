# K9PiAlarm

K9 Pi Alarm is a Python based Rasberry Pi Alarm System that monitors air temperature and displays it onto a screen.

The objective is to allow those with animals to monitor the temperature of a space and alert them when that space reaches levels they have set.
This is very much a work in progress, code is not optimized, pretty, but it does function on my test device. 

![Main Screen](https://user-images.githubusercontent.com/87459771/137964084-1bd78e60-e1ba-4933-966d-06d5b8687596.jpg)

## Items Required:
- Adafruit SHT-31 Temperature Sensors (x2)
- Raspberry Pi

## Items Recommended:
- Screen to view the temps, preferably touchscreen to interact with menus etc.

##Setup:
- Set up is fairly easy but does require manipulating some code at the moment. 
- Line 19, TempSensor2 is set to x44 for testing purposes, and needs to be changed to x45.
- Line 90 & 96 is the email/text alert setup and requires you to enter your sending and receiving email address for it to work. See https://github.com/kootenpv/yagmail for more info about yagmail. 

## Future Fixes / Patches / Features:
- Play Audio to alert you that the temperature has reached Warning Level, sleep for certain time, play audio again.
- Play a different audio file to alert you that the temperature has reached Alert Level and play continously until resolved.
- Alert via Email/Text that the Pi is using battery power (Power Source TBD) and lost main power.
- Currently the Camera Window functionality doesnt work. I intend to utilize Nest (Google) API camera to monitor inside the K9 Portion of the Vehicle, with the camera utilizing the truck WiFi. 


## Very Far Future / Need Help:
- Interface with a Vehicle via Bluetooth OBD to send commands when temperature reaches alert to roll down windows and set off car alarm.
- Some other way to alert a user (like a pager or beeper) that temperature has reached alert level. 
- UI Update to a cleaner more professional look

## Features Added
- Email / Text Alerts to notify you that the temperature has reached Warning / Alert Levels. (Requires Pi to have WiFi) 11/2/2021
