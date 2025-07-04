---
title: "OPEN-ESPilot"
author: "Tomas Kuchta"
description: "An OSHW, ESP32-based flight controller, built for affordability, flexibility!"
created_at: "2025-07-21"
---

**Total Time Spent: x** <!-- Going to figure it out when I'm done-->

## Written README.md - 21-6.2025
Like every begining of a Open Source project I create a GitHub repo and write a readme to let people know on what I'm working on.

**Time spent: 1.5h**

## Goal setting and asking for help and interest in the ardupilot comunity - 26.6.2025
I have written out a list of things I would need help with. And did simple goal setting to see if people like my idea.  
Then written a message and posted it on [ardupilot discussion forum.](https://discuss.ardupilot.org/t/help-me-build-the-first-open-source-esp32-flight-controller-for-makers/135974)  
Also I wanted to ask the devs on the Discord channel so I have also messaged them.  
I'm thankful for any help from the community as I have some perception but community needs can be other. When workng together we can make useful things for more people!

I have created Issues for each goal in this repo to keep ideas in one place.  
After that I have created issues for thing that needs to be decided on.  
I'm sharing my notes for the message in [asking for help and interest in the ardupilot comunity.md](https://github.com/Tomas-Kuchta-FPV/Open-ESPilot/blob/41703091e80cd6ef6a6719e9a7e344e687c4ec42/asking%20for%20help%20and%20interest%20in%20the%20ardupilot%20comunity.md)

**Time spent: 3h**

## Talked with DavidBuzz and asked for help, laid ground work for ESP32S3 core schematic and Pin definitions - 28.6.2025
I have read a lot of great responses to the message. Thank everyone for support.

We have decided on a form factor of a plane FC. Because this is my First FC and I didn't want to complicate it.  
David had an interesting idea to make it 30x30 Drone form factor. But that would need a two sided components and more than 4 layers. So that will hopefully be project for another day. I love this idea.

This sparked an idea of the first design constraints, which are Inexpensiveness, availability and hackability(flexibility)!

With the help of David we have decided on a MCU [ESP32-S3-WROOM-1-N8](https://lcsc.com/product-detail/WiFi-Modules_Espressif-Systems-ESP32-S3-WROOM-1-N8_C2913198.html?s_z=n_ESP32-S3-WROOM-1-N8).  
We think that you should be able to fit the AP code on 4mb flash but this project is aimed at more of a Dev board/Flight Controller hybrid so we were thinking of either 16mb or 8mb flash and no PSRAM as it isn't needed. And the 8mb hit that sweet spot of price and developer needs.  
He has also pointed me to his [pin definition](https://github.com/davidbuzz/ardupilot/blob/esp32s3-buzz-combined-sept-11th/libraries/AP_HAL_ESP32/README.esp32s3-pin-selection-hints.txt). And I have compiled the definitions into a spreadsheet.

He said that I completly forgot the SD card. So I have opened an issue for it.

Also I have deleted my work so I needed to recover it. 🤦 - Commit 6e2a837

Then I have edited the README.md to reflect the design constraints. To let everyone know about what is this project!

**Time spent: 4h**

## Finished the ESP32S3 and its peripherals and Finished Power side of things. - 30.6.2025
I started by researching how to implement the ESP32-S3 WROOM module. Since I’ve previously worked with the ESP32-C3, I already have some background knowledge.  
During this phase, I also learned about KiCad buses and hierarchical schematic design.

I have made the schematic with the MP1584 IC because I thought there are modules based on this IC but after desoldering the chip. It didn't really look like the correct footprint so I have deleted it because it would be too much work. ... I've said after I have made a schematic symbol and implemented it to the schematic with its components.

So I have decided to use the *Clone "MP1584" module* thats at least how do I call them. Because this way its way easier and probably cheaper as I would either need to either desolder the chip from the board or buy it separately. So Module will help a lot in terms of cost and simplicity.

So after all of that I have created another set of schematic symbol and footprint. This took tooooo looooong. At least it's done.

And made the schematic prettier. :]

![MCU Schematic](https://github.com/Tomas-Kuchta-FPV/Open-ESPilot/blob/main/Journal%20Images/MCU_Schematic.png)
![Power Schematic](https://github.com/Tomas-Kuchta-FPV/Open-ESPilot/blob/main/Journal%20Images/Power_Schematic.png)
![MCU Clone MP1584 module](https://github.com/Tomas-Kuchta-FPV/Open-ESPilot/blob/main/Journal%20Images/Clone_MP1584_module.jpg)

**Time spent: 5h**

## Added Schematic and footprint of the GY-91 IMU and implemented it to the schematic. - 1.7.2025
Today I haven't much time to work on this project so I had Just one goal of implementing IMU which is the GY-91 module.  
Its Going to be used as a module on the board because I'm implying same philosophy as for the *Clone "MP1584" module*.

I always like the schematic symbol creation in KiCAD. But creating the footprint is much more frustrating as I can't use normal CAD tools to constrain the footprint. I would love to make footprints in FreeCAD, maybe there is a better worflow?

![IMU](https://github.com/Tomas-Kuchta-FPV/Open-ESPilot/blob/main/Journal%20Images/IMU_Schematic.png)


**Check if the footprint is correct using a paper representation - 3.7.2025**
Today I haven't had much time so I only checked if the footprints I've made are correct by printing them on paper.  
But when exporting I've noticed that I forgor the front silkscreen. So this should be corrected when I have time.  
After printing the first sheet it printed in portrait and it was shrinked.  
Then I printed it in landscape and after confirming with calipers it was shrieked a little which didn't matter. Aleast I can check the proportions which seemed to be correct.

After checking everything seemed to be OK except for the F. Silkscreen.

![Custom Footprint](https://github.com/Tomas-Kuchta-FPV/Open-ESPilot/blob/main/Journal%20Images/Custom_footprint.jpg)

**Time spent: 2h**
