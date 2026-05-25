# English to Japanese on iDrive 6　・　iDrive6の英日言語設定
### Unlock Japanese Language on your *non JDM* F-Series BMW via BimmerCode

## Disclaimer! 
You are going to be coding values in KOMBI and HU_NBT_EVO. **Back up your data before changing values.**

## Purpose: 
The purpose of this guide is to help you unlock different languages in your F-Chassis BMW. While this guide specifically only unlocks Japanese, you could use this as a good starter to help you unlock other languages in your own car.
The car that was used in the testing of this guide is a 2018 BMW X1 F48, built for the Canadian market. This car does not have navigation nor touch screen (see picture below). 

<img width="1919" height="993" alt="image" src="https://github.com/user-attachments/assets/8ccd1de6-96d5-44d9-9b79-cf721737de74" />


## Prerequisites: 
- BimmerCode https://bimmercode.app/ (I used the Windows version of this app however the iOS/Android version will work too.)
- ENET Cable (I recommend using a wired ENET to Ethernet cable as opposed to a WiFi/Bluetooth Dongle.)
- **!!optional!!** Ethernet to USB-C/Lightning (In case you are doing this on your phone/laptop without a way to plug in the Ethernet.)

## Before we Code: 
- **I would recommend to code in the order that appears below.** 

## Preparing to Code:
1. Locate the OBDII port.
2. Plug the ENET Cable into the OBD port.
3. Connect the Ethernet cable to the device with BimmerCode.
4. Turn the ignition ON (Engine ON is also fine)
5. Connect the Car to BimmerCode.

##  Step 1. HU_NBT_EVO Coding (Headunit)
1. Enable Expert Mode.
2. Search for ```LANGUAGE```

<img width="1920" height="1140" alt="image6" src="https://github.com/user-attachments/assets/86f13c52-7b64-4297-9631-0004666a99b6" />

4. Set the following:
```
LANGUAGE_JAPANESE -> master
LANGUAGE_ENGLISH_UK -> list
LANGUAGE_ENGLISH_US -> nicht_aktiv
```

<img width="600" height="675" alt="image7" src="https://github.com/user-attachments/assets/361055bb-21dd-4ced-926e-cd3a72f96575" />
<img width="600" height="675" alt="image8" src="https://github.com/user-attachments/assets/efba6821-0414-4233-beb8-f33cc130bd75" />
<img width="600" height="675" alt="image9" src="https://github.com/user-attachments/assets/4e428b8e-f9d6-457a-91f9-b26b436181ff" />



4. Press code.

**!!! At this point, you will notice that the screen will reboot, and the iDrive display will be blank. Don't worry, we'll fix this below. !!!**


## Step 2. KOMBI Coding (Gauge Cluster/Meter Panel)
1. Enable Expert Mode.
2. Search or ```SPRACHE```

<img width="1920" height="1140" alt="image11" src="https://github.com/user-attachments/assets/c5d6227b-0004-4959-b382-117ada2c48ef" />


3. Set the following:
```
SPRACHE -> japan
```

<img width="600" height="675" alt="image12" src="https://github.com/user-attachments/assets/ac1a14e4-daa2-4029-aa75-33ff2eeb0e32" />


4. Press code.

**!!! You will probably see your gauge cluster flash. Don't worry. You will also see that the time and date has been reset, with Japanese displaying correctly on the gauge cluster but not on iDrive itself. We're almost done. !!**

## Step 3. HU_NBT_EVO Coding (Headunit)
1. Enable Expert Mode.
2. Search for ```COUNTRY```

<img width="1920" height="1140" alt="image13" src="https://github.com/user-attachments/assets/d714f750-f8d9-40f1-8f65-cef43dab9d0d" />


3. Set the following:
```
COUNTRY -> japan
```

<img width="600" height="675" alt="image14" src="https://github.com/user-attachments/assets/f501e73d-31f1-4981-83c8-3546f202f0d9" />


4. Press code.


## End result
If you followed this completely (and still have the legal disclaimer showing on startup), you will see: 

<img width="720" height="607" alt="image" src="https://github.com/user-attachments/assets/4ee1bbd3-3cfa-44a5-a669-e0ceec9ad35a" />

Your BMW's iDrive System is now set to Japanese. ここから日本語で安全運転をして下さい。 

## Next Steps
- In the HU_NBT_EVO coding menu, there are options for other East Asian languages such as Thai, Korean, Chinese, etc. I think it's possible to display these languages provided you set up the ```COUNTRY``` and ```SPRACHE``` flag to their appropriate values.  

## Resources: 
I'd like to thank these BMW owners for helping me look in the right direction. 
- https://f80.bimmerpost.com/forums/showthread.php?t=1350581
- https://www.bimmerfest.com/threads/time-and-date-gone-after-coding-kombi-language-on-f48.912184/
- https://mhhauto.com/Thread-Bmw-NBT-Language-Programming
- https://www.bimmerfest.com/threads/language-stuck-on-french-help.905226/
- https://f30.bimmerpost.com/forums/showthread.php?t=2077521

