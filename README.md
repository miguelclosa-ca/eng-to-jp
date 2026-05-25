# English to Japanese on iDrive 6
# (incomplete)
### Unlock Japanese Language on your F-Series BMW via BimmerCode

## Disclaimer! 
You are going to be coding in values in KOMBI and HU_NBT. **Back up your data before changing values.**

## Purpose: 
The purpose of this guide is to help you unlock different languages in your F-Chassis BMW. While this guide specifically only unlocks Japanese, you could use this as a good starter to help you unlock other languages in your own car.
The car that was used in the testing of this guide is a 2018 BMW X1 F48, built for the Canadian market. 

## Prerequisites: 
- BimmerCode https://bimmercode.app/ (I used the Windows version of this app however the iOS/Android version will work too.)
- ENET Cable (I recommend using a wired ENET to Ethernet cable as opposed to a WiFi/Bluetooth Dongle.)
- !!optional!! Ethernet to USB-C/Lightning (In case you are doing this on your phone/laptop without a way to plug in the Ethernet.)

## Before we Code: 
- **I would recommend to code in the order that appears below.** 

## Preparing to Code:
1. Locate the OBDII port.
2. Plug the ENET Cable into the OBD port.
3. Connect the Ethernet cable to the device with BimmerCode.
4. Turn the ignition ON (Engine ON is also fine)
5. Connect the Car to BimmerCode.

##  Step 1. HU_NBT Coding
1. Enable Expert Mode.
2. Search for ```LANGUAGE```
3. Set the following:
```
LANGUAGE_JAPANESE -> master
LANGUAGE_ENGLISH_UK -> list
LANGUAGE_ENGLISH_US -> nicht_aktiv
```
4. Press code.

**!!! At this point, you will notice that the screen will reboot, and the iDrive display will be blank. Don't worry, we'll fix this below.!!!**


## Step 2. KOMBI Coding
1. Enable Expert Mode.
2. Search or ```SPRACHE```
3. Set the following:
```
SPRACHE -> japan
```
4. Press code.
