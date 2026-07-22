## Log 1, 20-7-2026
I looked for better chips that could support ADC and more pins. The AtTiny-84A-20PU-AVR (AVR means it is rectangular) does just that, i went ahead and started making the schematic and i also researched if the new chip needs any special connections to ADC pin. I also learned about pin channels.
Port A pins support ADC, ADC stand for Analog-to-digital conversion, it turns signals from a sensor (thermistor, photoresistor) into data the chip can process.

I went for an Arduino-esque design since it had been the only microcontroller i used in real life (using pin-sockets for digital, analog, ground and power signals)

<img width="430" height="430" alt="image" src="https://github.com/user-attachments/assets/d087e9c1-55d2-43e7-ae23-735de19ef02a" />

## Log 2, 22-7-2026
I finished the schematic and started choosing footprints for the layout, i based my choice off of existing parts from the internet so that everything would fit (it didn't work out very well last time)
I chose 2 capacitors, 1 Micro-USB port, various pin sockets, 2x3 pin header and the ATTiny-84A-20PU chip (The PU part means it's a THT AVR chip)
