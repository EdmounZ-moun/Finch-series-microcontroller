## Log 1, 26-12-2025
Started research for the Finch V1 Devboard. This microcontroller uses the AT-Tiny85-20PU and a USB-C port for power transmission only, the data comes through an ISP-header, which is connected to the computer with an USBasp programmer. I thought i could use the USB port for the data too, but this chip does not support that.

I researched chip architecture and connections and i learned that there are a lot of types of chips and not all of them process information, for example, some chips such as the NE555 oscillator chip's sole purpose is to keep track of time.

Time spent: 3 hours

## Log 2, 6-1-2026
I made the schematic of the devboard using knowledge of pin connections. I tried to reverse engineer popular devboards such as the Arduino Uno to understand connections in practice, this did not work out because the Arduino is a multi-layer pcb, so i could not see all of the traces. I searched for the Arduino Uno schematic, this did work out well.
<img width="2117" height="1483" alt="image" src="https://github.com/user-attachments/assets/c7499f07-408e-4683-8ab8-60f998418853" />

Time spent: 2 hours

## Log 3, 7-1-2026
I tried making the PCB layout. It didn't work out multiple times and had to re-route the traces. It was quite hard to make a compact circuit board. I learned about trace thickness and PCB-Layers

## Log 4, 16-1-2026
Finalised the design and ordered the parts and PCB but when everything arrived i concluded that the USB-C port wouldn't work on this PCB for two reasons:
1. The USB-C port is connected to pads with SMD connections, i do not have the gear to solder SMD connections.
2. The port would not fit onto the board because mechanical pins were in the way and the pads on the port and PCB did not line up.
I decided to quit on this project for a bit.

Time spent: 1 hour

## Log 5, 22-5-2026
I revisioned my design by swtiching to Micro-USB with Through Hole solder connection and switched to GPIO pins instead of predetermined components, I retraced the PCB using better techniques to save space (e.g Ground Pour and shorter distances) A Ground Pour is using the entire empty space on a PCB for the ground plane. This is not very practical on compact boards such as mine, but i worked my way around this problem by adding the ground plane to the backside of the PCB where no components are situated, i also used thermal reliefs with every hole connection so the copper ground plane would not act as a giant heatsink. This way the solder will flow through. I also ordered the parts for this new iteration
<img width="385" height="388" alt="image" src="https://github.com/user-attachments/assets/2dc2e30f-2798-444c-9ea1-43a560e67f91" />
<img width="330" height="530" alt="Schermafbeelding 2026-07-21 000752" src="https://github.com/user-attachments/assets/ba208d07-c8c5-4013-b094-f86eda639dd9" /> 
(Ground is the blue part)

Time spent: 4 hours

## Log 6, -7-2026 (break because of school exams)
