# My-3.5mm-Earphones-got-Wireless-Bluetooth
I give my earphones a wireless audio transmitting power, Now I can plug any 3.5mm headphone/earphone and listen over bluetooth.

When it comes to Bluetooth audio, one company comes into mind id jieli also known as jerry tech. They provide a huge range of products starting from Bluetooth 3.0 to 5.0. I got my hands on one Bluetooth board from DF robot using the same IC. The main thing about this IC, that they provide great features in small form factor and low prices. There are a lots of different kinds of boards which comes with different specification and audio output you can browse DF Robot webpage and choose the best among them as per need.

In this tutorial we will make a universal Bluetooth for 3.5mm earphones, which can be directly plugged into board and can be controller wirelessly over Bluetooth. Nowadays most of the mobile phones and laptops do not have 3.5mm jack so it may be a great solution. Through the article we will discuss some newer Bluetooth technologies, PCB design, Circuit engineering, required components and problems with this board.

More about Jieli (jerry) Bluetooth:

They are the most popular manufacturer of DSP and Bluetooth chips. Most of the recent Bluetooth audio tech use their IC. The Jieli IC use high quality DSP and inbuilt audio amplifier for small earphone speakers. Sadly there is no open-source info, firmware, programmer and datasheets available. Some of the partner companies shared the datasheet but not the complete info about the microcontroller and DSP. If we want to change the name of Bluetooth, voice commands and program it is not possible.

Why 5.0 Bluetooth:

Bluetooth 5.0 offers significant improvements over older versions in terms of range, data transfer speed, and efficiency. With its longer range, devices can communicate up to 300 meters apart, reducing signal dropouts. The increased data transfer rate of up to 2 Mbps enables faster and smoother connections, enhancing audio quality and supporting high-quality audio streaming. Moreover, Bluetooth 5.0 consumes less power, prolonging battery life for devices. These advancements collectively make Bluetooth 5.0 a superior choice for more reliable, efficient, and versatile wireless communication.

Making the universal Bluetooth for 3.5mm headphones:

Universal means we can plug any 3.5mm headphones or earphones in this device and use them wirelessly. The good thing is that this module is plug on the other end so you can carry it easily in pocket. Most of the devices do not have any audio output jack nowadays, so we can connect the old earphone over Bluetooth and listen the pleasant 24bit DAC sound very clearly.

Components required:

DF Robot JIELI series Bluetooth 5.0 board

TP4056 charging board

300mah battery

Switch and Battery

Earphones or headphones

Custom PCB

https://jlcpcb.com/?from=SSA

Problems with this Bluetooth:

This board comes with great specification still there are some options which I think are missing. The charging IC is mandatory when working on this type of project. Using the separate charging module take more space and make the whole circuitry heavier. One push button is mandatory on the PCB to on/off the Bluetooth.

I combined all this things by soldering on top of the board which increase the overall thickness and weight a little bit. And a suitable battery is required to power up all the circuit, a big battery is not recommended but it should be rechargeable.

Solution by Redesigning the PCB:

The other solution to make this circuit smaller and more compatible is to add all the required components on a single PCB. It will reduce the overall formfactor increase the battery life and overall looks of the board. But it is very hard to redesign the PCB without any datasheet and components connection info. I tried to search everywhere but the datasheet of this specific IC is not open source. But I found some compatible circuits which are from the same company and circuit is given below for a reference. But I can't say anything without reverse engineering the original PCB.

In the next tutorial, I may reverse engineer this board and make a suitable connection diagram from that which may help me to modify the circuit and redesign the PCB. Turn Your Designs into Reality with JLCPCB – Your Trusted PCB Manufacturer. High-Quality PCBs at Unbeatable Prices. Fast Prototyping & Reliable Production. Join Thousands of Satisfied Designers Today!

JLCPCB is the most reliable PCB manufacturer from CHINA, get your 5pcs 2layer PCB just in $2. JLCPCB provides the huge range of services including stencil, PCBA, SMT assembly, 3D printing and Metal CNC.
https://jlcpcb.com/?from=SSA

Battery consumption:

The maximum power delivery is noticeably small, on full volume the max current consumption is around 40mA @5volts. So when connected with a Bluetooth device this taking only 0.2watts of power. But this IC can also be powered directly from 3.7v lithium polymer battery. Which increase the current consumption to 54mA. A little 300mah battery may last up to 5.5 hours of continuous stereo sound from both earphones.

This power rating depend on the type of earphone/headphone you are connecting to this board. Because the overall impedance may vary a little bit of each earphone so power delivery can be calculated as per that.

Using the Bluetooth as Audio Card:

This specific board from DF Robot can also be used as a digital sound card for PC. Just solder the pads given in the bottom solder layer of PCB. And connecting it via USB micro, PC detect the hardware as sound card. Now you can use this sound card to connect any headphone/earphone to any USB compatible system.

Like in most of the Raspberry Pi boards the analog audio output is not supported by the hardware. But connecting it to USB we can digitally record audio. Try JLCPCB now, Sign-up using this link and get free PCB coupons worth $54 (Applicable to new users only).

https://jlcpcb.com/?from=SSA
