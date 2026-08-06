## Log 1, 20-7-2026
I looked for better chips that could support ADC and contain more pins. The AtTiny-84A-20PU-AVR (AVR means it is rectangular) was perfect for my needs. I went ahead and started making the schematic and i also researched if the new chip needs any special connections to ADC pin. I also learned about pin channels.
Port A pins support ADC, ADC stands for Analog-to-digital conversion, it turns signals from a sensor (thermistor, photoresistor) into data the chip can process.

I went for an Arduino-esque design since it had been the only microcontroller i used in real life (using pin-sockets for digital, analog, ground and power signals)

<img width="430" height="430" alt="image" src="https://github.com/user-attachments/assets/d087e9c1-55d2-43e7-ae23-735de19ef02a" />

Time spent: 3 hours

## Log 2, 22-7-2026
I finished the schematic and started choosing footprints for the layout, i based my choice off of existing parts from the internet so that everything would fit (it didn't work out very well last time) I also used parts which i used in the previous devboard, so i did not need to order them again.
I chose 2 capacitors, 1 Micro-USB port, various pin sockets, 2x3 pin header and the ATTiny-84A-20PU chip. (The PU part means it's a THT AVR chip, other chip types include ARM and ESP)
I had to learn how to make my own footprint because the old one was removed somehow, luckily i had pictures so i could rebuild it from scratch.

Time spent: 1 hour

## Log 3, 23-7-2026
I started making the PCB layout, it was quite the same, but i stumbled upon a problem. I did not know which pin was the GND on the physical USB-Micro port, so my current footprint may be wrong and would cause the board to malfunction. I contacted the manufacturer but until then i will keep this design.

<img width="373" height="453" alt="image" src="https://github.com/user-attachments/assets/4c5c2405-60cf-40a4-9c12-ff807b524ef1" />

I will also need to change this on the Finch V1 if the footprint is wrong.

Routing was a bit harder with this board, mainly because of the larger amount of pins, luckily i had alot space on the bottom side of the board so i could route traces there if needed.
I did research on how a chip knows what type of signal it recieves: analog or digital

Time spent: 3 hours



