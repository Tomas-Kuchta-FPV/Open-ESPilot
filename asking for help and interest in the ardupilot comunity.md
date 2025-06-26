## Moto
An OSHW, ESP32-based flight controller, built for affordability and flexibility!
## Goals setting message
### Goals of this message 
- Straight foward
- kinda short
- mension higway to HW
- to set goals

### What goals needs to be set
- Going to figure out GPIO breakout in the process
- [ ] MCU
	- needs to be the Module
	- ESP32 vs ESP32S3
- [ ] Which INS
	- Gyro, Accelometer
	- Barometer
	- Magnetometer is it needed?
- [ ] UARTs
	- One for connecting to the PC
	- Two HW for pheripeal
	- Can we use SW UARTs
- [ ] Inverted Sbus input?
- [ ] Elrs reciever connector like on the speedy bee F405
- [ ] USB-C
	- On board
	- Off board
- [ ] Does it really need Power monitoring?
	Altleast voltage monitoring as It Isnt hard to integrate
- [ ] GPIO breakout
### What design decisions need to be checked
- 6 servo outputs

### Should also ask
- is it reallycheaper?
- are people interested?

### The message
Hi evheryone 👋,
I'm tying to develop an ESP32 based flight controller. The main focus being on affordability and a robust development platform.
I'm delveloping this under Higway to hardware.
I would like it to be Open Source so the comunity can build it together.
I don't have as much experience in this port. I haven't also designed a lot of PCB boards, but I should be able to work it out. :)
So please can you help me decide which components I should use. Once I have the schematic I will give an update and ask if somebody has an idea of what to improve.

To give you a basic outline of what I'm planning:
- ESP32/S3 module seems logical, as using the bare chip would be too difficult to implement
- Almost the feel of a professional FC board of the likes of SpeedyBee F405 WING APP or  Mateksys F405 WING
- It will be only one board
- There will be one BEC

And now for the questions that would help with goal setting
1. ESP32 vs ESP32S3 module?
2. Which INS I should use?
	- I think that we need Gyro, Accel, Gyro
	- We don't nesserly need a Magnetometer as there are on GPSs.
	- GY-90 Does have multiple chips
	- ICM20XXX it seems better for this. Also the Baro needs to be decided.
3. UARTs
	- One for connection to the GCS
	- And other two hardware ones for Connecting to pheripeals
	- Can we use SofwareSerial?
4. Reciever connection
	- ELRS connection via header
	- Should I include inverted Sbus input?
5. USB-C connector
	- Onboard?
	- Offboard? Like on the SB F405 Wing.
6. Power monitoring
	- Voltage is super simple using a resitor divider - Going to implement it
	- Current is harder and more expensive. Please help me decide if I should Implement it.
7. GPIO breakout
	- How many exposed GPIOs?
	- One idea I had is that we can make modules like ELRS, GPS and etc.
	- Which form factor either ESP devoard or a custom one
		- ESP devboard form factor would be nice as we can use the modules for other projects
8. Form factor/layout style:
	- Sudgestion from AI.
	- I’m not fully decided yet, but I’ll aim to make the board as compact as reasonably possible.
	- Planning to keep the shape rectangular for easier mounting and compatibility.

If you are a dev for ESP32 please let me know and hopefully in over a monh I'll have the prototype in my hand. If it all goes to plan I would love to send you some boards.


#### AI remake

Hi everyone! 👋

I'm working on a project to develop an ESP32-based flight controller, focused on being affordable, hackable, and a solid development platform.

This is part of the Highway to Hardware initiative, and I want it to be open-source, so we can build it together as a community. 🚀

I’m still learning – I don’t have a ton of experience designing flight controllers or PCBs yet – but I’m motivated and slowly figuring things out!

Right now, I’m at the component selection stage and I’d love to hear your thoughts. Once I finish the schematic, I’ll post an update and ask for suggestions on how to improve.

---

**🔧 Design Goals & Ideas**
- ESP32 or ESP32-S3 module – simpler than using bare chips
- Inspired by boards like SpeedyBee F405 Wing APP or Mateksys F405 Wing
- Single-board design with 1x BEC
- Modular – plan to support external ELRS, GPS, and possibly other modules via headers
- Aiming for a “dev board meets flight controller” hybrid


**Things I’d love input on:**

1. MCU
	- ESP32 vs ESP32-S3?
	- Which one is better suited for this? Especially considering performance and future proofness?

2. IMU/INS selection:
	- We'd definitely need Gyroscope + Accelerometer
	- Not sure if a Magnetometer is needed (GPS modules often include one)
	- Thinking of the ICM20XXX family over older combo boards like GY-90 as they have more chips
	- Also open to Barometer suggestions

3. UARTs:
	- Plan to use:
	- 1 for telemetry (GCS)
	- 2 for peripherals (GPS, receiver, etc.)
	- Is SoftwareSerial implemented or can it be used?

4. Receiver input:
	- ELRS header support like on the SB F405 WING
	- Should I also add an inverted SBUS input for compatibility?

5. USB-C connector:
	- Should the USB-C be onboard, like on most ESP32 dev boards?
	- Or offboard, like on SpeedyBee-style boards with a connector on a cable?
	- Or maybe a hybrid approach – onboard USB-C by default, but with solder pads available for hacking in an off-board connector if needed?

6. Power monitoring:
	- Voltage sensing via resistor divider is easy – will add
	- Current sensing is more complex and costly – should I include it?

7. GPIO breakout:
	- How many exposed GPIOs?
	- One idea I had is that we can make modules like ELRS, GPS and etc.	​- Which form factor either ESP devboard or a custom one
		- ESP devboard form factor would be nice as we can use the modules for other projects

8. Form factor/layout style:
	- I’m not fully decided yet, but I’ll aim to make the board as compact as reasonably possible.
	- Planning to keep the shape rectangular for easier mounting and compatibility.

---

📝 **Follow the Project**
You can track progress, view schematics, and join the discussion on GitHub:
👉 [Open-ESPilot Repository](https://github.com/Tomas-Kuchta-FPV/Open-ESPilot)
I’ll be posting regular updates there, including design files, dev notes, and future testing results. Feel free to open issues or share your ideas!

If you're into ESP32 dev or just excited about this sort of project, I’d love to hear from you!
If all goes to plan, I hope to have a prototype in hand within a month 🤞
And if things go well, I’d love to share a few boards with interested testers. 😊

I’m not a native English speaker, so I used AI (ChatGPT) to help me rephrase my original idea more clearly and friendly. The raw version is in my JOURNAL.md if you're curious. :)

Thanks for reading and helping shape this little adventure!

— Tomáš
