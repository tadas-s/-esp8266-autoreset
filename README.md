# FTDI cable adapter with dtrset reset method

Schematic taken from [this blog post][1]. The only small difference is output header pins drops
CTS and RTS pins and replaces with FLASH and RESET signals.

So board input is a standard FTDI 6 pin cable and output is:

    pin 1 -> GND
    pin 2 -> FLASH (to be connected to GPIO0)
    pin 3 -> VCC
    pin 4 -> TXD
    pin 5 -> RXD
    pin 6 -> RESET (to be connected to reset pin)

Project mentioned above exposes FLASH and RESET as a separate 2 pin header.

Schematic preview:

![schematic preview][2]

Complete and tested board:

![board][3]

Schematic captured and PCB done using the amazing [KiCad][1]!.

[1]: http://www.jce.lu/blog/?p=143 
[2]: autoreset-schematic-preview.png
[3]: board-photo.jpg
[4]: http://kicad-pcb.org/
