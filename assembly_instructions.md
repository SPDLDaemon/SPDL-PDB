# SPDL PDB Assembly Instructions

## tools needed
* soldering iron
* solder
* wire cutters
* wire strippers
* needle nose pliers
* multimeter
* small flathead screwdriver

## parts needed

* 1x PCB

* 1x set of components from [bill of materials](/BOM.csv)

* 2x tamiya connectors for batteries (with wires)

* 1x main power switch

* 1x fuse holder (with wires) and fuse

* 4 1-inch pieces of 18 AWG wire

* 2 batteries

## Time to Solder!

### TLV76150DCY: U5, U6

### TLV76133DCY: U3, U4

### leds: D1-D6, the long lead is the positive lead and goes in the round hole to the right for each led.

### 0.1uF (104) capacitors: C1, C3, C6, C7

### 10uf capacitors:

C2: positive lead is on the right near the mounting hole

C4: positive lead is on the left farther from the edge of the board

C5, C8: positive leads are on the right closer to U5 and U6

### 680 ohm resistors: R1, R3

### 1k ohm resistors: R2, R4, R6

### 3.3k ohm resistor: R5

### Diode: D10, the banded end is the negative end and goes in the square hole on the left while the positive end goes in the round hole labeled A

### 3 header pins: 3 sets of 3 for NT1 and 1 set of 3 for NT2

### 4 header pins: J25, J26

### Molex 254 2 pin connector: 5V

### small switch: SW1

### buck converters: U1, U2
use 90 degree header pins FID1-FID4, trim the pins so that they don't touch each other

also use 4 wires to connect the IN+ and OUT+ wires

![buck converter wiring](/assembly%20photos/regulatorPins.jpg)

### JST XH 3 pin connectors: J1-J16

### Molex 254 3 pin connectors: J17-J24

### Screw terminal blocks: J28-J31 for 14v, J32-J33 for battery, main1 for main switch

![assembled board](/assembly%20photos/photo1.JPG)

## Turning on the PDB for the first time

Connect the wires of the tamiya plugs to the battery screw terminals, making sure to connect the positive wire to the positive terminal and the negative wire to the negative terminal.

Solder wires to the main power switch

Connect the main power switch to the MAIN SWITCH screw terminal. Polarity doesn't matter for the switch.

Connect the fuse holder to the FUSE screw terminal. Polarity doesn't matter for the fuse.

Make sure that the three jumpers for NT1 and NT2 are not installed.

Make sure that the main power switch is off.

Make sure that the 5V switch is off (towards the edge of the board).

Plug charged batteries into the tamiya connectors.

Turn on the main power switch. If there is smoke turn the switch back off.

Use a multimeter to measure the voltage between TP-U1 and the ground wire on the left of the board. 

Adjust the screw on the U1 voltage regulator until TP-U1 is at 6.0 volts.

Use a multimeter to measure the voltage between TP-U2 and the ground wire on the left of the board.

Adjust the screw on the U2 voltage regulator until TP-U2 is at 5.0 volts (or whatever voltage you want to supply to your servos and any other components you connect to the molex connectors).

Turn the main power switch back off.

Plug the three jumpers into NT1 and NT2. Placing them all in the leftmost position is recommended, but check the [user guide](/218PDBguide.drawio.png) for more information on the different jumper settings.

Turn the main power switch back on. If there is smoke turn the switch back off.

All 6 lights should be on at similar brightness. You can use a multimeter to check that all the pins are supplying the correct voltages.

Turn the main power switch back off.

Turn the 5V switch on and check that D1,D2,D3,D4 are on and that D6 is off.

Turn the PDB back off (and remember to turn it off whenever you are working on your circuit).

### Congrats, your PDB is ready to use!
