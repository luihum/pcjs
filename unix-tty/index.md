---
layout: page
title: UNIX Computer with VT100
permalink: /unix-tty/
redirect-from: /devices/unix-cool-tty-secret-redirect
machines:
  - id: unix-pc
    type: pcx86
    name: IBM PC AT CGA 16Mb
    config: machine.xml
    connection: pc-serial-1->vt100.serialPort
  - id: vt100
    type: vt100
    name: DEC VT100
    config: vt100.json
    layout: ../_includes/vt100.html
    connection: serialPort->unix-pc.pc-serial-1
---

This is a test of a VT100 terminal connected to a IBM PC AT running UNIX System V. The serial ports are *virtually* connected, so the VT100 
should be available as a tty once you finish installing System V and get out of single-user mode.

If the terminal becomes LOCKED, press the SET-UP key twice to unlock it. 

{% include machine.html id="unix-pc" %}

{% include machine.html id="vt100" %}
<!--   -->
