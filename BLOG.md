# Build blog
After building it halve a year ago it didn't work right out of the gate. So I threw it into a drawer to comeback to it later.  
https://mastodon.social/@TomasKuchta/115453693371285049  
https://mastodon.social/@TomasKuchta/115457650264164261  
https://mastodon.social/@TomasKuchta/115462604233771055  
https://mastodon.social/@TomasKuchta/115462624371600031  

And HackClub take two have sparked another spark in me to continue. After all that trouble...  
SO I've written everything down on a piece of paper and I'll also transfer it here.  
I have hooked it up to an external PSU with monitoring on the 3V3 rail. And it wsowed me that it drew 30mA of curent with 5V provided by the USB port and 50mA when the USB was unplugged. Wiedrd you may think.  
And when I was unplugging it I have started with the 3V3 ground which is also the PEN neutral line. And after unpluging it I've noticed the dreaded magic smoke. And I have quickly disconected the USB power. I's probably because of a ground loop.  
Yeah and the 5V supply is shorted. Wait didn't I put PTC fuze there? nope, another thing to the list of problems.

List of things that went wrong:  
- [ ] Add a note to remove the 2k2 pullups on the GY-91 as they were backfeeding the 3V3 line through the ESP
  - [ ] Add a note about the pullups to the schematic
- [ ] Invertor should have a 3V3 pullup insted of a 5V one as ESP is 5V intolerant
- [ ] Think about adding a backfeed diode to the 3V3 line
- [ ] USB-C port should only power the core (ESP)
- [ ] 5V regulator: instead of a fiddly potenciometer it should be removed and in designator R3 a 4k5 0402 should be addded. With 4k53 being ideal.
- [ ] 3V3 line should get a lover voltage zener diode as the current one is not doing anything
- [ ] Think about using a mosfet for the invertor instead of a BJT tranzistor to lower cost
- [ ] Fix the anoying buzzer somehow
- [ ] Add a PTC fuze as I think it's missing
