---
permalink: /about_wheeldash/
title: "About WheelDash"
excerpt: "WheelDash is a standalone app for Garmin devices."
last_modified_at: 2024-02-08
toc: true
author_profile: false
author: BlkFri
---

If you want to support this project, visit my <a href="https://ko-fi.com/wheeldash" target="_blank" rel="noopener noreferrer">ko-fi page</a>!
{: .notice--info}

## A few words about WheelDash

This project started as a personal project to meet my needs with my EUC. I wanted a simple and efficient app that would allow me to avoid using both my phone and my watch (if my watch has GPS and supports BLE, why use a third-party app on my smartphone?), have a PWM alarm management, and allow me to record my rides, all for free.

As a longtime Garmin user, I decided to develop a Garmin app for my EUC. Once I had a version that was usable for everyday use, I decided to release the source code for the app as well as publish a release of WheelDash on the Garmin store. The first feedback I received gave me the desire to continue the adventure a little further, so I decided to continue development, supported by the encouragement of a handful of people. While I am the only developer, WheelDash has benefited from the exchanges I have had with the first users. It is a project developed by and for the EUC rider community that we are. This is also why I want WheelDash to be and remain 100% free and open source.

in 2024, Garmin modified it's Bluetooth stack and since then, all Garimin user who have decided to upgrade their watch are observing increased latency in information updates.  Garmin not listening to its app developers, I have decided to create a new version of WheelDash for Amazfit.  In addition to making much cheaper watches, their bluetooth implementation rocks allowing real time updates of critical information such as the reported PWM. I still maintain the Garmin version but most new features now land Amazfit.

## Features

WheelDash is an app for Amazfit and Garmin devices and offers real-time display of important data such as speed, battery level, temperature, PWM, and various other metrics. It also allows for the management of common wheel settings directly from the watch. In addition, it provides alarms for PWM, speed, and temperature, and allows you to map specific actions on your watch button (like toggling your EUC lights on or off).

On Garmin, It seamlessly integrates with the Garmin environment, making it easy to record your rides and store data transmitted by your wheel. All route information and ride data are readily accessible through the Garmin Connect app or portal.

On Amazit, there is no such enviroment so I decided to develop a web server which can be used to securely upload your rides and consult the detailed stats online.

WheelDash is a standalone app and not a companion for WheelLog, DarknessBot, or EUC World, so WheelDash does not require any of these apps to function.  As on option, you can use WheelDash to display information sent by EUC World.

## Versions

On Garmin WheelDash exists in two forms: a Garmin application and a datafield that can be added to an existing activity. While the application and datafield versions share a fair amount of code, the datafield version is more restricted due to Garmin's restrictions on memory usage and UI refresh rate. The datafield version is however THE solution to be able to use Garmin native navigation and display or record wheel related data.

<center>
<img src="/assets/images/WD_AppTypeTab.png"/>
</center>

## Compatible EUCs

WheelDash currently supports all EUCs model from the following brands :

- Gotway/Begode/Extreme Bull
- Leaperkim
- KingSong
- Inmotion (recent models starting from V11)
- Nosfet

<center>
<img src="/assets/images/WD_EUC_CompatTab.png"/>
</center>

**Note:** The KingSong S22 (and potentially the S16 and S19) uses a Bluetooth module incompatible with most Garmin smartwatches. It's only been confirmed to work seamlessly with the Forerunner 255.
{: .notice--warning}

## Compatible Garmin Devices

WheelDash is compatible with most BLE-enabled devices that support CIQ version 3.1 or later. If your watch isn't listed in Connect IQ or you're unable to find VESCDash, please feel free to contact me with information about your watch model.

**Note:** Garmin has recently made changes to their Bluetooth stack, which has resulted in increased lag and disconnection issues on several of their smartwatches, particularly the Fenix 7 and Epix series. Unfortunately, there's currently no solution to this problem that I can provide. One potential workaround is to downgrade the watch firmware, but this may have other trade-offs or limitations.
{: .notice--warning}

You can check watch models specification here:

[https://developer.garmin.com/connect-iq/compatible-devices/](https://developer.garmin.com/connect-iq/compatible-devices/)

## Compatible Amazfit devices

- Active 2 (Round or Square, with or wthout NFC)
- Balance 2 (Round or Square)
- Bip 6
- T-Rex 3

## Activity Recording

WheelDash allows you to track your riding session by saving it as a Garmin activity or as sessions on Aamazfit. Besides saving your ride route, it also records the following metrics of you EUC :

Speed, PWM, Voltage, Current,Motor power and motherboard temperature.

Additional metrics are also available in your activity summary : trip distance, maximum speed, maximum PWM, maximum Current (App only), maximum power (App only), min/max temperature (max on App only), average speed, average power (App only), min/max voltage, min/max battery % (max on App only)

Note : Due to memory restrictions in datafields, less metrics are available in the activity summary in WheelDash: datafield.
