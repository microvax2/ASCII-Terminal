For firmware, please visit: https://github.com/dhansel/TerminalUSB/

For convenience, I have placed a copy of V1_3 firmware here [2021].

Credits go to David Hansel

08-MAY-2021: 
BACKSPACE/DELETE does not work on a DEC VAX console. Therefor main.c has been fixed to send the correct code ("\177") for BKSP.
file: main.c
line: 140
line: 141
