# 🚁 Open-ESPilot

**An open-source ESP32-based flight controller to bring the power of ArduPilot to *everyone*!**

Hi there, and welcome to **Open-ESPilot**! 🎉
This is a work-in-progress open hardware project to create a low-cost, hackable flight controller (FC) based on the mighty [ESP32](https://www.espressif.com/en/products/socs/esp32). Whether you're a developer, hacker, drone enthusiast, or curious builder — this is for you!

We're on a mission to make running [ArduPilot](https://ardupilot.org/) more accessible on everyday hardware.

> 🚀 This project is part of [Hack Club’s *Highway to Hardware*](https://highway.hackclub.com/), a program that empowers students to build awesome electronics projects. Big thanks to them for their support!

---


## Why Open-ESPilot?
I wanted to take on the challenge of designing a **cheap, open-source, and hack-friendly flight controller** — and share the journey with the community!

> To the best of my knowledge, this is the first-ever community-made ESP32-based flight controller built specifically for ArduPilot — a true one-of-a-kind platform!

- A reference platform for running ArduPilot on ESP32
- A starting point for others to remix, improve, and explore
- Fully open-source, modular, and *actually fun* to tinker with


## Project Status
🔧 **This project is in its early design & experimentation phase.** Nothing is final yet, and contributions or feedback are very welcome!  
I have finilized the PCB and going to send it to higway to get a grant to build it.  
![PCB Render](https://github.com/Tomas-Kuchta-FPV/Open-ESPilot/blob/main/Images/PCB_Render.png)  
![PCB Screenshot Front](https://github.com/Tomas-Kuchta-FPV/Open-ESPilot/blob/main/Images/PCB_Screenshot.png)  


## Core Design Ideas 💡
- *Dev board meets flight controller* hybrid
- Ultra low cost — 2-layer, single-sided PCB to keep it budget-friendly
- Readily available components
- Hackability so you can hack on your own features
    - Maybe modules?! (eg. ELRS, GPS)
- ❤️ Designed with care by and for the community


### 🛠️ Planned Features
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
This flight controller is built to run the [ESP32 port of ArduPilot](https://ardupilot.org/dev/docs/esp32-autopilot.html) — a massive shoutout to the incredible developers and contributors who made this possible! 
> This project wouldn’t exist without them — go show them some love!

## My background
I previously built a basic ESP32-based FC that worked — but it wasn’t as polished as dedicated hardware. After testing with the SpeedyBee F405 Wing APP for an ArduPilot Rover, I had the idea to make a more focused and community-driven board.


## Built With
- [ESP32](https://www.espressif.com/en/products/socs/esp32) – the core micro controller
- [KiCad](https://kicad.org/) – for PCB design
- [ArduPilot](https://github.com/ArduPilot/ardupilot) – the autopilot software we're building for
- ❤️ Open source tools and community support
- ... and Love ❤️


## 🤝 Contributing
Ideas, suggestions, or just curious? Feel free to open issues, PRs, or reach out! This project is made to be built with the community.

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

The price is for the qantity.  

## 🏁 License
Hardware: [CERN-OHL-W](https://ohwr.org/cern_ohl_w_v2.txt)

Firmware: Ardupilot


## 🙏 Thanks
Thanks to the amazing folks at [Hack Club](https://hackclub.com/) for supporting student hardware projects through *Highway to Hardware* 💥

And big thanks to the ArduPilot community for keeping robotics open and awesome.
