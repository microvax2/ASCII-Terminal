# ASCII-Terminal
VT-100 Clone ASCII Terminal

VT100-Clone ASCII Terminal on a chip, this project is a new PCB designed around "Geoff's VT100 Terminal" by Geoff Graham, and the modified firmware designed by David Hansel  (https://github.com/dhansel/TerminalUSB) @dhansel which supports a USB Keyboard.

Also inspired by Peter Hizalev's work @petrohi (https://github.com/petrohi/terminal).

What is changed in this project is:

* SMT components used (except for the connectors, which I preferred to keep mechanically sound)
* The footprint is compatible with a VESA mount, so the PCB can be mounted directly to the rear of a VGA monitor using VESA mount screw holes (M4) 
* Removed PS/2 connector
* A standard type A USB connector, so a standard USB keyboard can be connected without any adaptors
* A USB 3.0 20-pin Header, for connecting a keyboard using a PC-style USB 2.0/3.0 front panel
* A 4-pin Molex ("Disk Drive") connector for powering the board from a PC-type power supply
* A 2.5mm DC jack connector for powering the board from a 5VDC wall wart power supply
* 3 DIP switches for selecting the baud rate
* 3 Solder bridges for selecting the text color (R/G/B)

The USB 3.0 header makes it possible to place the project in a PC Case, and connecting it to the front panel using the 20-pin USB 3.0 loom. Then, the PC case will become a "terminal housing": it will accept a USB keyboard on its front panel.

Please note: for a working terminal, not all the options need to be assembled:

* You need a type A USB connector (J7) *or* a 20-pin USB 3.0 header (P6), but probably not both
* You need to supply 5V power from P2, *or* from J1, *or* from J6, you need only one of them assembled
* If you need VGA output assemble J3. If you need Composite video output, assemble P3
