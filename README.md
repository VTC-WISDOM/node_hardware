# hardware
a collection of schematic and pcb designs for the WiSDOM node
unless otherwise specified, everything contained in this repository is licensed under the CERN Open Hardware License version 2 - Weakly Reciprocal License (CERN-OHL-W).
this is comparable to the gpl2, see LICENSE for details

## Using this repo
using your favorite package manager, install kicad-footprints and kicad-symbols alongside kicad. this is the best way to get the standard libraries. if you for some reason cannot do so, see the linked official kicad libraries in kicad-libs/footprints and kicad-libs/symbols.
in the kicad symbol editor, go to preferences -> manage symbol libraries and select "add existing", navigate to the kicad-libs/symbols directory and select the symbol libraries contained therein. repeat this with the symbols contained in kicad-libs/JLCPCB-Kicad-Library.
repeat this for footprints.

### node-rp2040
stores all of the relevant design files for the WiSDOM node that is based on the RP2040

### node-rp2350
like above but the RP2350

### other
test projects, antenna and transmission equipment, etc. anything unspecified

### docs
will add as much documentation as possible!

## Node V6 (RP2040)

changes:
- removed 5v regulator
- changed rp2040 xtal to the recommended part due to availability
- changed the sim card slot due to availability
- reviewed other parts and made changes to ensure full availability from both JLC and Digikey
- changed footprints over to JLC library footprints
- major layout changes- pin headers now broken out in two halves, etc - look at the pcb for a full description
- removed jst connectors (evil) and replaced them with barrel jacks
- mounting holes now m2.5 instead of m2

## Node V5 (RP2040)
 ***SIM7080G NON-FUNCTIONAL***

change since previous version:
- added USBLC6 esd protection on the usb line
- added CAT24 eeprom ic
- removed options for rtc to stick with just the PCF8523
- added SP3485 for RS485 / MODBUS communication
- added u.fl connector for the ism radio
- changed to narrower profile pushbuttons for run/bootsel
- added additional reset switch to interrupt 3.3V to the board entirely (used to reset the device to a known state for all components including the radios)
- yet more improvements to routing
- updated design to be mostly assembled by JLC pcb fab available components 
