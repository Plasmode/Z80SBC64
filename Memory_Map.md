# Z80MB64 and Z80SBC64 Memory, I/O map
## Memory Map
The memory is consists of 128K of RAM in four 32-K banks:

Top 32K of RAM is the common memory. The bottom 32K can be bank selected by writing to bank select register at I/O location 0x1F as follow:

- 0x0 is normal operation
-0x1 do not use
- 0x2 is for bank 0 of CP/M-3
-0x3 is the reset value where the top 32K of physical memory is mapped to 0x0-0x7FFF
## I/O Map
### UART
A hardware receiver is implemented in CPLD with the following I/O addresses:

- Read-only serial data receive register at 0xF9
- Read-only serial receive status register at 0xF8 where
  - D[0] is the receive ready flag, 1 indicates data is ready, 0 indicates no data
- Write-only bit-bang transmit register at 0xF9
  - The content of D[0] appears on the TX output pin. D[0] is high at reset. Software must “bit-bang” D[0] of transmit register to emulate the serial port transmit function.
### Compact Flash Registers
Compact flash registers are 0x10 to 0x17

###mBank Select Register
Bank select register is write only located at 0x1F

bu
