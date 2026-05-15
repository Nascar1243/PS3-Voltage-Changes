# PS3-GPU-Overclock
The VID Tables map the Hex value needed to program the SYSCON EEPROM to select the coresponding voltage for mullion or sherwood syscon. Be sure to use the correct table for your model of PS3. 

SYSCON EEPROM Addresses these apply to:

Sherwood = 0x51 for RSX and 0x50 for Cell

Mullion = 0x3111 for RSX and 0x3110 for Cell
    
Note: The default value is FF on retail consoles. Writing FF to these addresss will revert RSX Core to stock voltage.

Note: VER-001 (Lxx and Pxx) use the Mullion voltage table, there isn't an explanation why but that is how it works.

The 01_patch_rsx_oc.tcl file is a modified version of the dropdown in MFW Builder, which adds more overclock timings. Place it into the "tasks" folder of MFW Builder, overwriting the one in there. Since it adds so many more combinations it may take a few seconds longer for the dropdown to appear after checking the box to enable the overcolck. 
