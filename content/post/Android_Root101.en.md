+++
title = "A Guide to Flashing Custom ROMs [Android]"
slug = "Flashing Custom ROMs 101"
date = "2018-02-25T00:00:00"
description = "Sick and tired of the bloatware on your current OEM ROM. Head over and learn how to flash custom ROMs."
author = "RohanVTK"
+++

**_(This blog starts off with a warning: Although the process is super easy and there hardly is a chance that you will brick your device during the process but, it's my responsibility to make you aware of it)_**

The guide would be inclined more towards Xiaomi devices as I own one and have worked with it. But, all other devices follow the same process, so go ahead and give it a read.

* To start off with, you should have a unlocked bootloader.

    **_For Xiaomi devices refer to the following link : [Click-Here](https://en.miui.com/unlock/)_**

    Follow the process and you'll surely have an unlocked bootloader in no time.
*(Although it might take some time for Xiaomi to process your request but thereafter it's a really fast process)*

* **_Download ADB(Android Debug Bridge) and Fastboot files from this link: [Click-Here](http://rootjunkysdl.com/files/?dir=Adb%20Fastboot%20Files)_**

    A .zip file for Windows will be downloaded. Extract these files to a folder.

* **_Next, download twrp recovery file(a `.img` file). Make sure that the twrp file is downloaded from here: [Click-Here](https://twrp.me/Devices/)_**

Place this file inside the folder created after extraction.

**_Make sure that the ADB, fastboot, recovery file and the rest of the files are placed inside the same folder._**

* Now download a ROM of your choice. *(I personally use AOSP Extended ROM, it's pretty stable and is really performant when compared to other ROMs).*

    **_Link to AOSP Extended: https://www.aospextended.com/_**

* Also, download google apps .zip file.

    **_Link to OpenGapps: https://opengapps.org/_**

* Now open up the command prompt on Windows with **_adminitrator priviliges_**.
    
    _(To do this press the Windows key on your keyboard and search 'cmd' right click when command prompt comes up and chose 'Run as Administrator')_

* Now go the directory where the files you downloaded have been stored.
    if you don't know how to use Command Prompt

> `cd <dirname>` is use to go up a directory

> `cd..` is used to go down one directory


Finally pick your phone up and go to the fastboot mode, two methods have been listed below use any:

    1. Reboot to Bootloader ->(Hold Power + Volume down)

    2. Connect your phone to the PC after enabling the ADB debugging mode in the developer settings

> type `adb devices` if your device shows up then,

> type `adb reboot-bootloader`

Now to check that your device has entered the fastboot mode and is connected to the system _(connect your phone to the system if you followed method 1 mentioned above)_

> type-in `fastboot devices` if your device shows up then,

> type-in `fastboot flash recovery <nameOfTheRecoveryFile.img>`

Flashing would be done within a few minutes.

*So, the tough part's over.* :D

Moving on. 

> type-in `fastboot boot <nameOfTheRecoveryFile.img>`

Now the TWRP recovery opens up.

Transfer the ROM & Gapps file to the phone storage and click on install in TWRP recovery.

Find the .zip files.

Install the ROM and thereafter install Google Apps from the .zip file.

_After completing the process make sure to clear the Dalvik Cache and Cache memory._

_Reboot the Device._

**_Congratulations! Now you have a phone with a CUSTOM ROM of your own choice with no bloatwares._**

______
______

*If during the process you encoutered any issues do look up your issues on XDA or else Google your issues, you'll surely find a solution.*

*If you enjoyed reading this article do let me know by tweeting to me on my __twitter-handle @RohanVTK__. Your input will highly appreciable as well.*

*If you encouter any dead links do tweet about it, the links will be updated.*
