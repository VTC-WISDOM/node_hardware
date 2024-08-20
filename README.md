## hardware
a collection of schematic and pcb designs for the WiSDOM node

# V4
v4.0.2: schematic split into sheets for organization
        added better switching circuit for usb/bat operation. replaced 3.3V supply with a linear regulator for stability and reverse voltage protection. 
        includes first prototype of footprints for cellular interface. cellular functionality is not guaranteed until further testing.
        better layout of RP2040 traces. added jst connectors for battery and external power(labeled solar).
        
        only "v4\_0\_2" files will be tested. assume others should not be used.

# V3
v3.0: never built. don't use.
v3.1: discovered issue with RP2040 crystal, requiring 1k series resistance
v3.2: discovered issue with switching between external and battery power causing the RP2040 to enter a locked state.
      troubleshooted MCP7940 RTC and determined it will not communicate with the RP2040 for unknown reasons
      added 5.1k resistors on usb-c cc lines
      battery & power circuitry is insufficient and risks damaging pc usb outputs if battery is reversed. no overcharge protection
      retired, do not use

# V2
v2: second prototype, used only for testing radio communications. 
    retired, do not use

# V1
v1: initial prototype. retired, do not use
