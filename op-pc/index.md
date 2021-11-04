---
layout: page
title: IBM PC AT (Model 5170) with 32Mb RAM and 62Mb HDD
permalink: /op-pc/
machines:
  - id: ibm-5170-vga-op
    type: pcx86
    config: machine.xml
---
{% include machine.html id="ibm-5170-vga-op" %}

# IMPORTANT

This computer is a experiment to make a pretty OP computer. It currrently has:

   * CPU: 80386 @ 4MHz
   * RAM: 32MiB
   * HDD: 62MiB
   * 2 floppy drives
   * 1 CD-ROM drive
   * mouse
   * VGA 
   * 2 serial ports
   * 1 parallel port
   * a debugger
   
  Please note that mouse emulation is a bit slow.
  Also, if your computer can emulate close enough to the target speed, you can overclock the machine by clicking on the speed button.
 
 1. Make sure the PC DOS 3.30 Disk 1 floppy is inserted on drive A:. If not, insert it.
 2. Start the CPU with the Run button.
 3. The clock should already be correct; press Enter twice.
 4. To use the hard drive: 
      `FDISK`
       1
       1
       Y
       a
       Enter
       Enter
       `FORMAT C:`
       Y
       <Wait about a minute. Pro tip: Overclock the machine with the "4.00 MHz" button.>
       `SYS C:`
       `C:`
       `MKDIR DOS`
       `COPY A:*.* C:\DOS`
       `COPY B:*.* C:\DOS`
    This will only use half the hard drive due to a DOS bug. You can try another version to fix it.
