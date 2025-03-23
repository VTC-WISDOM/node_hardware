# hardware
a collection of schematic and pcb designs for the WiSDOM node
everything contained in this repository is licensed under the CERN Open Hardware License version 2 - Weakly Reciprocal License (CERN-OHL-W).
this is comparable to the gpl2, see LICENSE for details

## repo structure
### kicad-libs submodule:
this submodule stores the official kicad schematic, footprint, and 3d model libraries as well as unique parts and logos for WiSDOM and a further submodule for JLC preferred parts. licenses are contained within. this is intended to be used as the exclusive set of (project-specific) libraries for any WiSDOM kicad project

### node-rp2040:
stores all of the relevant design files for the WiSDOM node that is based on the RP2040

### node-rp2350
like above but the RP2350

### other
test projects, antenna and transmission equipment, etc. anything unspecified

### docs
will add as much documentation as possible!

## Current: Node V5 (RP2040)

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