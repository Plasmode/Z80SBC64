# Pictorial Assembly Guide for Z80SBC64
The sequence of soldering is start from the lowest height components to the tallest components. This keeps the components pressed against the pc board as the soldering progress.

**Bare PC board, component side**
![blank](Z80SBC64_blank_top.jpg)

**Bare PC board, solder side**
![solder](Z80SBC64_blank_solder.jpg)

**Resistors, SIP resistor and bypass capacitors are soldered first**
![resistor](Z80SBC64_resistor_top.jpg)

**Next the IC sockets are soldered**
![socket](Z80SBC64_socket_top.jpg)

**DS1210 is soldered directly to the board because the clearance between pin 1 of DS1210 and the battery holder is too tight to allow a socket.**
![battery](Z80SBC64_battery_top.jpg)

**The serial port connector and RC2014 bus connector are soldered next.**
![serial](Z80SBC64_serial_top.jpg)

**The headers for Altera programming and Bootstrap mode are soldered next.**
![jtag](Z80SBC64_jtag_top.jpg)

**EPM7064 PLCC44 socket, power jack, push button, and voltage supervisor are soldered next**
![plcc](Z80SBC64_PLCC_top.jpg)

**The 44-IDE adapter board is soldered last.**
![all](Z80SBC64_complete_top.jpg)

The assembly is completed. The board should be cleaned with isopropyl alcohol and inspected before adding components. Altera EPM7064 should be inserted first and programmed before others are added.
