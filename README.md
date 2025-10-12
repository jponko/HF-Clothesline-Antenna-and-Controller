# A Motorized Remote Controlled Clothesline Antenna for the HAM HF Bands 
![Figure 3](ClothslineLayout.png)

The basic layout of the clothsline antenna is shown in figure 3 above. Basically you move the feedpoint to match the antenna to the transceiver rather than trying to match the tranceiver to the antenna. I've made a few changes such as using 450 Ohm ladder line to the shack instead of the 300 Ohm twinleed. I'm using a 1:4 balbal in combination with a 1:1 current balun instead of the 6:1 balun shown. These transformers are built according to instructions from TRX Lab videos on Youtube and work very well. I'll be using short runs of 75 Ohm coax from my Kenwood TS-520 and TS-820 tranceivers. The TS-520/820's manual notes that it can effectively transfer power with an antenna system that results in an input impedance between 15 and 200 ohms.

### Remote and Motor Control
The remote and motor control use NodeMCU 1.0 ESP-8266 dev modules. The motor control uses a DIY rotary encoder using a PCB 120mm diameter disk with 36 apertures, a pair of photo interruptors,  and a 12V 45 RPM gear motor which I found at the Surplus Center. The Surplus Center has about 780 of these gear motors still in stock for $9.95 each as of October 2025.

You'll also need silicon covered #12 AWG wire with a high strand count which gives it its flexability. Mine is about 4.5mm in diameter and has about 100 strands. I don't have a source for the wire as I bought 300 feet of of this wire from a vendor on Aliexpress about five years ago.

The zip file contains all the information and files needed to build a clothesline antenna. There are Arduino sketches, KiCAD (V9.x) PCB layout files for the boards and rotor disk. This includes the Gerber zip files in the production folders for sending to a PCB board maker. I used JLPCB to make mine.

https://www.kicad.org

You'll also need some type of box to mount the rotary encoder/NodeMCU in and feed it with 12V power. I'm using a case from a 1990's hard drive enclosure and a 12V 5A AC power adapter. 

The remote control uses a low power 5v supply. Barrel jacks are used on both devices.

I'll be putting the antenna up this fall on a 40 foot flag pole. So more info on how it actually performs will be comming soon. In the meantime, here are some photos of the remote control and motor control.

#### Remote
![Remote](remote.jpg)

![Remote](remote-front.jpg)
The SSD1306 OLED is epoxied to the pcb using plasticmstandoffs UV light epoxy. 

![Remote](remote-back.jpg)

#### Motor Control and Rotary Encoder
![MotorControl](encoder.jpg)

![MotorControl](mc-cover.jpg)

![MotorControl](mc-front.jpg)

![MotorControl](mc-back.jpg)

The roller guides are from an old VCR. The opening will get a plastic cover.

![MotorControl](mc-side.jpg)

The gear motor sticks out of the case but is waterproofed  with a pill bottle.
The two waterproof limit switches are shown in the foreground. They will be mounted on the front. Disks on the wire will activate the switches to stop the
gearmotor.

