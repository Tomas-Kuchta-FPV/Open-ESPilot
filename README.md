# Open-ESPilot

**An open-source ESP32-based flight controller designed to bring ArduPilot to more people.**

I welcome you to Open-ESPilot repo! This is a work-in-progress project to create a simple, open hardware flight controller (FC) based on the ESP32. It's being built with the goal of making it easier and cheaper to run [ArduPilot](https://ardupilot.org/) on accessible hardware — whether you're a developer, hacker, or just someone who loves robots and drones.

This project is being developed as part of [Hack Club’s *Highway to Hardware*](https://highway.hackclub.com/) program 🚀 Many thanks to them!


## Why this exists

Most flight controllers out there are expensive, closed-source, or hard to modify. At the same time, ArduPilot is one of the most powerful autopilot stacks out there, and the ESP32 is a super capable, low-cost microcontroller with built-in Wi-Fi that can be used for MAVlink.

So... why not bring them together?

The goal is to make a board that:

-  Create a reference platform for ArduPilot on ESP32.
-  Make it easy and affordable to build or buy.
-  Keep it fully open-source, modular, and easy to hack.


## ⚙️ Project Status

I previously built a basic ESP32-based FC that worked — but it wasn’t as polished as dedicated hardware. After testing with the SpeedyBee F405 Wing APP for an ArduPilot Rover, I had the idea to make a more focused and community-driven board under *Highway to Hardware*.

🔧 **This project is in its early design & experimentation phase.** Nothing is final yet, and contributions or feedback are very welcome!


### Core Design Ideas 💡

- Single PCB (stacked boards likely unnecessary)
- Modular thinking: support for swappable or optional components (ELRS, ESCs, etc.)
- Needs to be **inexpensive** but flexible — if it’s pricier than commercial options, it should offer something unique or valuable
- ❤️ Designed with care by and for the community

### 🛠️ Planned Features

- [ ] Basic schematic and PCB layout

- [ ] The component selection is decided in [Issues](https://github.com/Tomas-Kuchta-FPV/Open-ESPilot/issues)

- [ ] Compare BOM cost to commercial FCs

- [ ] Complete documentation and build guide
- [ ] 3D-printable case/enclosure


## Design Phases

1. **Planning & goal setting**
2. **Schematic design**
    - Start with core ESP32 + power
    - Add sensors and outputs
    - Evaluate BOM & gather feedback
3. **Community feedback loop**
4. **PCB layout**
5. **Prototype ordering**
6. **…And hopefully it works on the first try! 🤞**



## Pin assigment
Big **TBD**
> Adapted from: [Random Nerd Tutorials - ESP32 Pinout Reference](https://randomnerdtutorials.com/esp32-pinout-reference-gpios/)

| GPIO | Used for    | Notes | Input     | Output | Pin Notes                                                                      |
| ---- | ----------- | ----- | --------- | ------ | ------------------------------------------------------------------------------ |
| 0    | Boot Button |       | pulled up | OK     | outputs PWM signal at boot, must be LOW to enter flashing mode                 |
| 1    |             |       | TX pin    | OK     | debug output at boot                                                           |
| 2    |             |       | OK        | OK     | connected to on-board LED, must be left floating or LOW to enter flashing mode |
| 3    |             |       | OK        | RX pin | HIGH at boot                                                                   |
| 4    |             |       | OK        | OK     |                                                                                |
| 5    |             |       | OK        | OK     | outputs PWM signal at boot, strapping pin                                      |
| 6    |             |       | x         | x      | connected to the integrated SPI flash                                          |
| 7    |             |       | x         | x      | connected to the integrated SPI flash                                          |
| 8    |             |       | x         | x      | connected to the integrated SPI flash                                          |
| 9    |             |       | x         | x      | connected to the integrated SPI flash                                          |
| 10   |             |       | x         | x      | connected to the integrated SPI flash                                          |
| 11   |             |       | x         | x      | connected to the integrated SPI flash                                          |
| 12   |             |       | OK        | OK     | boot fails if pulled high, strapping pin                                       |
| 13   |             |       | OK        | OK     |                                                                                |
| 14   |             |       | OK        | OK     | outputs PWM signal at boot                                                     |
| 15   |             |       | OK        | OK     | outputs PWM signal at boot, strapping pin                                      |
| 16   |             |       | OK        | OK     |                                                                                |
| 17   |             |       | OK        | OK     |                                                                                |
| 18   |             |       | OK        | OK     |                                                                                |
| 19   |             |       | OK        | OK     |                                                                                |
| 21   |             |       | OK        | OK     |                                                                                |
| 22   |             |       | OK        | OK     |                                                                                |
| 23   |             |       | OK        | OK     |                                                                                |
| 25   |             |       | OK        | OK     |                                                                                |
| 26   |             |       | OK        | OK     |                                                                                |
| 27   |             |       | OK        | OK     |                                                                                |
| 32   |             |       | OK        | OK     |                                                                                |
| 33   |             |       | OK        | OK     |                                                                                |
| 34   |             |       | OK        |        | input only                                                                     |
| 35   |             |       | OK        |        | input only                                                                     |
| 36   |             |       | OK        |        | input only                                                                     |
| 39   |             |       | OK        |        | input only                                                                     |

## Built With

- [ESP32](https://www.espressif.com/en/products/socs/esp32) – the core microcontroller
- [KiCad](https://kicad.org/) – for PCB design
- [ArduPilot](https://github.com/ArduPilot/ardupilot) – the autopilot software we're building for
- ❤️ Open source tools and community support


## 🤝 Contributing

Ideas, suggestions, or just curious? Feel free to open issues, PRs, or reach out! This project is made to be built with the community.


## 🏁 License

Hardware: [CERN-OHL-W](https://ohwr.org/cern_ohl_w_v2.txt)

Firmware: Ardupilot


## 🙏 Thanks

Thanks to the amazing folks at [Hack Club](https://hackclub.com/) for supporting student hardware projects through *Highway to Hardware* 💥

And big thanks to the ArduPilot community for keeping robotics open and awesome.
