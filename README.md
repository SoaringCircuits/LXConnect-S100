# LXConnect S100

## General remarks
This small board is designed to simplify and organize the wiring in your glider.
It provides a clean extension point to wire the cables for the LX S100 standalone variometer, reducing clunky connectors hanging free.

![board](https://github.com/SoaringCircuits/LXConnect-S100/blob/master/docu/LXConnect-S100.png)

## Electrical installation
Installation is easy, but some basic skills in creating cable harnesses are needed to create the connection from S100 to the board.
While the S100 uses a D-Sub-15, the board uses a D-SUB-15HD to save space.
The following diagram shows the harness to build to connect S100 and board. 


The board provides terminals for power, the switching inputs (SC, VP, IN1-4, OAT), as well as a connector for the CAN-Bus with optional terminator directly on the board.

## D-SUB Connectors
The board uses two D-SUB connectors, one for the connection to the S100 and one for the CAN-Bus.
I recommend to use connectors with crimped contacts for both connectors, but solderd ones will work as well.
All connections are direct lines, there is no need to crimp/solder more than one cable to a single contact.

## CAN-Bus and terminator
The LX S100 provides a CAN-Bus to connect external devices like a remote stick, flap indicator, etc.
The end of the Bus has to be terminated by a 120 Ohm resistor.

Originally LX provides a big D-SUB Connector with such a resistor to be plugged at the end of the bus.

This board provides a resistor with a solder jumper to properly terminate the bus if no external devices are connected, saving space and free hanging cables and connectors.
If the onboard terminator should be used, just close the jumper by soldering it together.

## Wago Terminals
All terminals are easy to operate, just push the actuator with a little screwdriver and push-in or pull-out the conductor.

The terminals for fuses and devices are suitable for various types of wires:
- Solid concductor 0.2 - 1.5 mm^2
- Fine-stranded conductor 0.2 - 1.5 mm^2
- Fine-stranded conductor with ferrule 0.25 - 1.0 mm^2

The terminal for the main supply can handle conductors up to:
- Solid concductor 0.1 - 4.0 mm^2
- Fine-stranded conductor 0.1 - 4.0 mm^2
- Fine-stranded conductor with ferrule 0.25 - 2.5 mm^2

## Mechanical installation
The half housing is 3D-printed and reliably protects against short circuits on the contacts on the underside of the board.
With four mounting holes for M3 screws, the board can be securely and firmly mounted in the aircraft, with the screws fixing both the housing and the board at the same time.

## Disclaimer
Installation and use of the board are the sole responsibility of the user.
LXnav, the manufacturer of the S100, is and was NOT involved in the development of the board and can not be hold responsibly for any failures or damage to the device.
The board has been built to the best of my knowledge and belief, but no warranty or guarantee can be given for correct functioning or interference immunity.
The legal usability must be checked before each individual installation and, in case of doubt, clarified with competent and authorized personnel (CFS).

## Licence
Copyright Fabian Schöttler 2025.

This source describes Open Hardware and is licensed under the CERN-OHL-P
v2 or later.

You may redistribute and modify this documentation and make products
using it under the terms of the CERN-OHL-P v2 or later (https:/cern.ch/cern-ohl).
This documentation is distributed WITHOUT ANY EXPRESS OR IMPLIED
WARRANTY, INCLUDING OF MERCHANTABILITY, SATISFACTORY QUALITY
AND FITNESS FOR A PARTICULAR PURPOSE.
Please see the CERN-OHL-P v2 for applicable conditions

## Contact
If you have any questions or suggestions about the board, please send an e-mail to fabian@schoettlerhome.de.

------
Electrical, PCB and case design by [ScotteC](https://github.com/ScotteC)
