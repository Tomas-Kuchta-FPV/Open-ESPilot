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


## 🏁 License
Hardware: [CERN-OHL-W](https://ohwr.org/cern_ohl_w_v2.txt)

Firmware: Ardupilot


## 🙏 Thanks
Thanks to the amazing folks at [Hack Club](https://hackclub.com/) for supporting student hardware projects through *Highway to Hardware* 💥

And big thanks to the ArduPilot community for keeping robotics open and awesome.
