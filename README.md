# 6 Key Macro Pad

Footprints from https://github.com/tmk/keyboard_parts.pretty and https://github.com/egladman/keebs.pretty

Components used from https://github.com/tmk/kicad_lib_tmk

Built with SMD components, and ATMega32u4.

![build image](https://github.com/EriicLii/6-key-Macro-Pad/blob/master/Images/completed.jpg)

PCB:
![PCB Image](https://github.com/EriicLii/6-key-Macro-Pad/blob/master/pcb.png)

Schematic:
![Schematic](https://github.com/EriicLii/6-key-Macro-Pad/blob/master/schematic.png)

## Update 7/31
Finally got to soldering the parts. 
Had an issue with discovering the DFU. At first I though the microcontroller didn't come with the HWBE bit set from factory. However after painstakingly soldering the MOSI, MISO and SCK pins, then setting the fuses through ISP -- still no dice. I finally noticed that I hadn't wired VBus to VCC in my schematic. I guess I got taught the lesson of measuring thrice before sending it to fabrication.

QMK firmware setup was very easy. Kudos to everyone involved in the project as the abundance documentation and organization made it simple to get a new keyboard firmware set up. Right now I only have the option to manually change the keymaps in QMK then recompile. I'll perhaps attempt to make a Via keymap later as well. (Also I need to add pictures of the build!)

## Update 8/2
Added some pictures. You can see how I had to wire VCC to the Vbus pin on the back of the board.

![back image](https://github.com/EriicLii/6-key-Macro-Pad/blob/master/Images/solderedBack.jpg)
