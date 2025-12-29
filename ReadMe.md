# Parallel I/O, SASI Controller and R-Bus Interfaces Expansion Board for the Cypher Z80/68k SBC

This repository documents the hardware expansion board that I had designed and built for the [Motel Computers Cypher Z80/68000 SBC](https://github.com/rcl9/Cypher-Z80-68000-Single-Board-Computer-1984-by-Motel-Computers---History-and-Documentation) in 1986.

<div style="text-align:center">
<img src="/Images/Expansion board #1.jpg" alt="" style="width:70%; height:auto;">
</div>

It provided this additional functionality:

- A SASI port interface for the Shugart 1610-3G SASI controller card. SASI was the pre-cursor to the SCSI hard disk interface standard.

- A "R-Bus" or "Rob's Bus" interface. This was the high-speed bus protocol that I had designed for my multi-card DSP-based music synthesis computer named "Pegasus-II".

- A "Universal Parallel I/O Port" connector. This was my own parallel port standard that I had designed into all of my self-built 1980's Z80 computers. It allowed for my [out-board peripheral projects](https://github.com/rcl9/Imagery-of-Past-Projects) to be easily moved from machine to machine, before the advent of the USB protocol many decades later (such as for my EPROM emulator, OmniProm programmer, ZAP-A-Pal programmer, among other devices). 

- An Apple Macintosh SCSI interface based on the NCR5380.

The full set of schematics can be found in the schematics sub-folder.

## The "Universal Parallel I/O Port"

During the 1980's I standardized on this DB25 connector pinout for my "Universal Parallel I/O Port" which I used to interface with all of my [out-board peripheral projects](https://github.com/rcl9/Imagery-of-Past-Projects). 

| Bit # | Description| Printer Usage  |
| :-----: | :---: | :---: |
|1 | Ground| |
|4 | Data Out 7| Data strobe to printer |
|5 | Data Out 6| |
|6 | Data Out 5| |
|7 | Data Out 4| |
|8 | Ground| |
|10 | Data In 0| |
|11 | Data In 2| |
|12 | Data In 4| Paper out from printer |
|13 | Data In 6| Select-In from printer |
|14 | +12v| |
|15 | +5v| |
|16 | Data Out 0| |
|17 | Data Out 1| |
|18 | Data Out 2| |
|19 | Data Out 3| |
|20 | +5v| |
|22 | Data In 1| |  
|23 | Data In 3| |
|24 | Data In 5| Error from printer |
|25 | Data In 7| Busy from printer |

The output pin assignments were made compatible with the Exidy Sorcerer's DB25 parallel port connector. 
