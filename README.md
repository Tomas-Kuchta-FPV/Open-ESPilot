# Open-ESPilot

This is a community-driven hardware project focused on creating an open and accessible Flight Controller (FC).   
With the main focus on being on low-cost, availability and hackability!  

Most of the Ardupilot FCs on the market are released by qite a huge brands aren't OS and they cost a lot.  
Thats why I've started this project to make a Open source and low-cost FC with the comunity.  

The target firmware being [ArduPilot](https://ardupilot.org/), which is a powerfull open-source autopilot system.  

## Core Design Ideas
- *Dev board meets flight controller* hybrid
- Keep it budget-friendly
- Readily available components
- Hackability so you can hack on your own features
- ❤️ Designed with care by and for the community


## What are the goals
The main one being a reference platform for devs and hackers. Then we can then move to a product for the wider public.  

With the main focus on Hackability and Openness there are endless possibilities for creativity!  
Here are few ideas:
 - Prototyping and experimetation  
 - A low-cost alternative for those priced out of commercial FCs  
 - Teaching control theory and autonomous systems in schools  

## Why did I make it
I have a lot of experience with FPV drones running betaflight.  

Then I started playing with ESP32 based ardupilot for almost three years. All of then was for a competetion called Robotem Rovne.  
 - First one being an autonomous rover which was breadboarded together. As with any other breadboard project the wires were loose, they didn't make contact and the were faling off.  
 - Then I made a seccond rover with a FC soldered on a proto board. Which worked wonderfully!  
 - Then I tried to make a PCB with brushed motor controller. Not going to talk about this one. Didn't go to plan. :(  
 - After that I've bought a SpeedyBee f405 WING FC and mounted it to a RC car. This is my Ardupilot learning platform.  

And we are here as the SB FC sparked an idea to make a ESP32 Flight Controller into a universal PCB. Which wasn't done a lot.  

OH it seems like a Microsoft release cycle. Hope that this project won't end in disaster.


## Future development
This is the first FC I made with the help of the comunity so huge thanks to *everyone*. ♥️

### Ideas for future
 - modular system (eg. ELRS, GPS modules)
 - 30x30 FC for FPV drones. Thats harder as there are plenty of great cheap FCs


## Project Status
**I have the PCB made and now I need to order everything and test it!**
| PCB                                                                                                           | Render                                                                                          |
| ------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| ![PCB Screenshot Front](https://github.com/Tomas-Kuchta-FPV/Open-ESPilot/blob/main/Images/PCB_Screenshot.png) | ![PCB Render](https://github.com/Tomas-Kuchta-FPV/Open-ESPilot/blob/main/Images/PCB_Render.png) |


### The Plan
- [x] Basic schematic and PCB layout
- [x] Selection of components is decided in [Issues](https://github.com/Tomas-Kuchta-FPV/Open-ESPilot/issues)
- [ ] Compare BOM cost to commercial FCs - going to figure it out when I have time.
- [ ] Complete code, documentation and build guide


## Design Phases
1. **Planning & goal setting**✅
2. **Schematic design**✅
    - Start with core ESP32 + power
    - Add sensors and outputs
    - Evaluate BOM & gather feedback
3. **Community feedback loop**✅
4. **PCB layout**✅
5. **Prototype ordering**
6. **…And hopefully it works on the first try! 🤞**


## Firmware
We are now focusing on [ArduPilot ESP32 port](https://ardupilot.org/dev/docs/esp32-autopilot.html), they are making inredible work and the project wouldn't exist without their hard work.  
I won't be able to write the code by myself so huge props to the contributors! Thats why I'm focusing on the HW.  
There are also possibilites for you to write your own code.  


## Contributing
We would love to hear feedback. We are open to everything including issues, ideas and sudggestions.  
Thats why this project is Open Source.


## BOM
| Category      | Qty | Price (USD) | Description           | Link                                                                                                                                                           |
| ------------- | --- | ----------- | --------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| PCB component | 1   | 0.9         | TMB12A05              | https://lcsc.com/product-detail/Buzzers_Huaneng-TMB12A05_C96093.html                                                                                           |
| PCB component | 14  | 0.46        | 100nF                 | https://lcsc.com/product-detail/Multilayer-Ceramic-Capacitors-MLCC-SMD-SMT_YAGEO-CC0805KRX7R9BB104_C49678.html                                                 |
| PCB component | 7   | 0.11        | 22uF                  | https://lcsc.com/product-detail/Multilayer-Ceramic-Capacitors-MLCC-SMD-SMT_Samsung-Electro-Mechanics-CL21A226MQQNNNE_C5674.html                                |
| PCB component | 1   | 0.53        | 1000uF                | https://lcsc.com/product-detail/Aluminum-Electrolytic-Capacitors-SMD_ROQANG-VT1A102M0810_C311227.html                                                          |
| PCB component | 1   | 0.57        | 1000uF (Leaded)       | https://lcsc.com/product-detail/Aluminum-Electrolytic-Capacitors-Leaded_AISHI-ERR1VM102G20OT_C398835.html                                                      |
| PCB component | 1   | 0.57        | SS34                  | https://lcsc.com/product-detail/Schottky-Diodes_MDD-Microdiode-Semiconductor-SS34_C8678.html                                                                   |
| PCB component | 2   | 0.98        | PDZVTR5.1B            | https://lcsc.com/product-detail/Zener-Diodes_ROHM-PDZVTR5-1B_C253499.html                                                                                      |
| PCB component | 1   | 0.84        | B5819W                | https://lcsc.com/product-detail/Schottky-Diodes_MDD-Microdiode-Semiconductor-B5819W_C64885.html                                                                |
| PCB component | 1   | 0.49        | WS2812B LED           | https://lcsc.com/product-detail/RGB-LEDs-Built-in-IC_XINGLIGHT-XL-5050RGBC-WS2812B_C2843785.html                                                               |
| PCB component | 1   | 0.22        | Ferrite Bead          | https://lcsc.com/product-detail/Ferrite-Beads_TDK-MPZ2012S101AT000_C15957.html                                                                                 |
| PCB component | 1   | 0.87        | USB-C Receptacle      | https://lcsc.com/product-detail/USB-Connectors_Korean-Hroparts-Elec-TYPE-C-31-M-12_C165948.html                                                                |
| PCB component | 1   | -           | MP1584 module (clone) | https://www.aliexpress.com/item/1005005870392716.html                                                                                                          |
| PCB component | 1   | -           | GY-91                 | https://www.aliexpress.com/item/32652866365.html                                                                                                               |
| PCB component | 1   | 0.6         | AO3401A               | https://lcsc.com/product-detail/MOSFETs_AOS-AO3401A_C15127.html                                                                                                |
| PCB component | 2   | 0.45        | BC847                 | https://lcsc.com/product-detail/Bipolar-BJT_Nexperia-BC847B-215_C57668.html                                                                                    |
| PCB component | 2   | 0.21        | 5.1k                  | https://lcsc.com/product-detail/Chip-Resistor-Surface-Mount_YAGEO-RC0805FR-075K1L_C84375.html                                                                  |
| PCB component | 2   | 0.19        | 10k                   | https://lcsc.com/product-detail/Chip-Resistor-Surface-Mount_YAGEO-RC0805FR-0710KL_C84376.html                                                                  |
| PCB component | 1   | 0.21        | 1k                    | https://lcsc.com/product-detail/Chip-Resistor-Surface-Mount_YAGEO-RC0805FR-075K1L_C84375.html                                                                  |
| PCB component | 5   | 0.19        | 10k                   | https://lcsc.com/product-detail/Chip-Resistor-Surface-Mount_YAGEO-RC0805FR-0710KL_C84376.html                                                                  |
| PCB component | 2   | 0.49        | 10R                   | https://lcsc.com/product-detail/Chip-Resistor-Surface-Mount_YAGEO-RC0805FR-0710RL_C96347.html                                                                  |
| PCB component | 1   | 0.41        | 0.5mΩ                 | https://lcsc.com/product-detail/Chip-Resistor-Surface-Mount_Viking-LR12FTDR0M50_C37635712.html                                                                 |
| PCB component | 4   | 0.19        | 1k                    | https://lcsc.com/product-detail/Chip-Resistor-Surface-Mount_YAGEO-RC0805FR-071KL_C95781.html                                                                   |
| PCB component | 2   | 0.63        | Push Button           | https://lcsc.com/product-detail/Tactile-Switches_ALPSALPINE-SKRKAEE020_C115357.html                                                                            |
| PCB component | 1   | 5.14        | ESP32-S3-WROOM-1-N8   | https://lcsc.com/product-detail/WiFi-Modules_ESPRESSIF-ESP32-S3-WROOM-1-N8_C2913198.html                                                                       |
| PCB component | 1   | 0.87        | AMS1117-3.3           | https://lcsc.com/product-detail/Voltage-Regulators-Linear-Low-Drop-Out-LDO-Regulators_Advanced-Monolithic-Systems-AMS1117-3-3_C6186.html                       |
| PCB component | 1   | 0.41        | AMS1117-3.3 (Alt)     | https://lcsc.com/product-detail/Voltage-Regulators-Linear-Low-Drop-Out-LDO-Regulators_Slkor-SLKORMICRO-Elec-AMS1117-3-3_C880752.html                           |
| PCB component | 1   | 2.84        | INA219                | https://lcsc.com/product-detail/Current-Sense-Amplifiers_TI-INA219AID_C1574856.html                                                                            |
| PCB component | 1   | 1.32        | Micro SD Card Slot    | https://lcsc.com/product-detail/SD-Card-Memory-Card-Connector_HRS-DM3AT-SF-PEJM5_C114218.html                                                                  |
| PCB component | 50  | 0.46        | Pin Header (5x10)     | https://lcsc.com/product-detail/Pin-Headers_BOOMELE-Boom-Precision-Elec-2-54-1-10P_C57369.html                                                                 |
| PCB component | -   | 13          | Shipping              | -                                                                                                                                                              |
| PCB           | -   | 10.72       | PCB cost              | https://cart.jlcpcb.com/quote?orderType=1&homeUploadNum=4c39875b107d460986bfa4ef1bf68f70&businessType=example&fileName=Open-ESPilot_50.6x71.1mm_for_JLCPCB.zip |
| **TOTAL**     | -   | 50.97       | -                     | -                                                                                                                                                              |


## Built With
- [ESP32](https://www.espressif.com/en/products/socs/esp32) – the core MCU
- [KiCad](https://kicad.org/) – for PCB design
- [ArduPilot](https://github.com/ArduPilot/ardupilot) – the autopilot software we're building for
- ❤️ Open source tools and community support
- ... and Love ❤️


## License
Hardware: [CERN-OHL-W](https://ohwr.org/cern_ohl_w_v2.txt)

Firmware: Ardupilot


## Thanks
Many thanks for the amaizing people that make [Hack Club](https://hackclub.com/) possible.
Thanks to Hack Club for interesting so much people I don't know the numbers but maybe around thousants.  
Most of them are probably going to get a carier from it. Love your work! ❤️  

And big thanks to the ArduPilot community for keeping robotics and autonomy Open and hackable.
