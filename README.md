# PS3-GPU-Overclock
The VID Tables map the Hex value needed to program the SYSCON EEPROM to select the coresponding voltage for mullion or sherwood syscon. Be sure to use the correct table for your model of PS3. 

SYSCON EEPROM Addresses these apply to:

Sherwood = 0x51 for RSX and 0x50 for Cell

Mullion = 0x3111 for RSX and 0x3110 for Cell
    
Note: The default value is FF on retail consoles. Writing FF to these addresss will revert RSX Core to stock voltage.

Note: VER-001 (Lxx and Pxx) use the Mullion voltage table, the explanation is due to the VER boards using the same vid controller as mullion boards, making the Sherwood and Mullion monikors useless.  Basically if you use a VER, only use the Mullion voltage table.
