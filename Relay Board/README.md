# Relay Board for the IO Pi Plus 2.1 #

This is a 16 channel relay board suitable for use with the [IO Pi Plus version 2.1 from AB Electronics UK](https://www.abelectronics.co.uk/p/54/IO-Pi-Plus).  The board is compatible with the Panasonic JS series of single pole double throw relays and will work with relay coil voltages from 5V to 24V. 

The relay board is compatible with the following relays:

- JS1-5V-F
- JS1-6V-F
- JS1-9V-F
- JS1-12V-F
- JS1-18V-F
- JS1-24V-F

To build the relay board you will need the following parts:

- 16 x Panasonic JS series relays (model numbers listed above)
- 3 x ULN2003A darlington arrays (16 pin DIP package) 
- 1 x 20 pin IDC PCB connector (2.54mm pitch) 
- 16 x 3 pin 5mm screw terminals or other compatible connector. (5.08mm will also work)
 
The 20 pin IDC connector uses the same pin configuration as the [IO Pi Plus 2.1](https://www.abelectronics.co.uk/p/54/IO-Pi-Plus) so you can connect the two together using two 20 pin IDC connectors and a ribbon cable.  The relay numbers match the pin numbering on the IO Pi Plus bus making it easy to control the relays using our IO Pi software libraries.

To power the relay coils you will need a separate power supply that matches the voltage of the chosen relays.  ULN2003A Darlington arrays are used to switch the relays from a low voltage logic input.

The PCB dimensions are **100mm x 150mm**.  Gerber files are included in the project folder and use a file name format compatible with several PCB manufacturers including [iTead](https://www.itead.cc/open-pcb/pcb-prototyping/2layer-pcb-larger-than-10cm-x-10cm.html) and [Elecrow](https://www.elecrow.com/services/pcb-prototyping/5pcs-2-layer-pcb.html).  The “Gerber Files.zip” file contains a zip of the gerber files that can be uploaded directly to the PCB manufacturer of your choice.
The schematic and PCB files are included in Diptrace format, you can download a free version of Diptrace from [http://diptrace.com/download-diptrace/](http://diptrace.com/download-diptrace/)


----------


**Note:** The relay board can be used with older versions of the IO Pi Plus, [IO Pi Zero](https://www.abelectronics.co.uk/p/71/IO-Pi-Zero) and original IO Pi but you will need to only connect the 16 control pins on the IDC connector.  The ground pin will need to be connected separately to the GND pin on the IO Pi board as earlier models did not include the ground on the IDC header.  The relay numbers will also not match up to the outputs on the IO Pi.
