---
title: "OPEN-ESPilot"
author: "Tomas Kuchta"
description: "An OSHW, ESP32-based flight controller, built for affordability, flexibility!"
created_at: "2025-07-21"
---

**Total Time Spent: x** <!-- Going to figure it out when I'm done-->

## Written README.md
Like every begining of a Open Source project I create a GitHub repo and write a readme to let people know on what I'm working on

**Time spent: 1.5h**

## Goal setting and asking for help and interest in the ardupilot comunity
I have written out a list of things I would need help with. Then writen a message and posted it on [ardupilot discussion forum.](https://discuss.ardupilot.org/t/help-me-build-the-first-open-source-esp32-flight-controller-for-makers/135974)

Also I wanted to ask the devs on the Discord channel so I also written a message to them.

I'm thankfull for any help from the comunity as I have some perception but comunity needs can be other. When workng together we can make usefull things for more people!

I have created Issues for each goal in this repo to keep ideas in one place.

I'm sharing my notes in [asking for help and interest in the ardupilot comunity.md](https://github.com/Tomas-Kuchta-FPV/Open-ESPilot/blob/41703091e80cd6ef6a6719e9a7e344e687c4ec42/asking%20for%20help%20and%20interest%20in%20the%20ardupilot%20comunity.md)

**Time spent: 3h**

## Talked with DavidBuzz and asked for help, laid ground work for ESP32S3 core schematic and Pin definitions
I have read a lot of great responses to the message. Thank everyone for support.
I have decided on a form factor of a plane FC. Because this is my First FC and I didn't want to complicate it.
David had an interesting idea to make it 30x30 Drone form factor. But that would need a two sided components and more than 4 layers.
This sparked an idea of the first design constraints, which are Inexpensiveness, availability and hackability(flexibility)!
We have decided on a MCU [ESP32-S3-WROOM-1-N8](https://lcsc.com/product-detail/WiFi-Modules_Espressif-Systems-ESP32-S3-WROOM-1-N8_C2913198.html?s_z=n_ESP32-S3-WROOM-1-N8).
We think that you should be able to fit the AP code on 4mb flash but this project is aimed at more of a Dev board/Flight Controller hybrid so we were thinking of either 16mb or 8mb flash and no PSRAM as it isn't needed. And the 8mb hit that sweet spot of price and developer needs.
He said I forgot the SD card. So I have opened an issue for it.
David has pointed me to his [pin definition](https://github.com/davidbuzz/ardupilot/blob/esp32s3-buzz-combined-sept-11th/libraries/AP_HAL_ESP32/README.esp32s3-pin-selection-hints.txt). And I have compiled the definitions into a spreadsheet.
Also I have deleted my work so I needed to recover it. 🤦 - Commit 6e2a837
Then I have edited the README.md to reflect the design constraints.

**Time spent: 4h**
