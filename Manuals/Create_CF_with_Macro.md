# Creating a new CF disk for Z80SBC64 and Z80MB64 with a TeraTerm Macro
For people with Z80SBC64 and Z80MB64: attached is a TeraTerm Macro and files that allow you to install CP/M software in a new CF disk. This is the macro I ran when I want to create a new CF disk. Unzip and place all files in c:\teraterm\newcf; then run the macro “NewCF.TTL” in TeraTerm. It will perform the following tasks:

1. Run RAM diagnostic for 5 seconds
2. Format drives A:, B:, C:, D: <–please note all previous files will be erased
3. Install CP/M2.2 BDOS/CCP/BIOS
4. Install CP/M 3 CPMLDR
5. Install SCMonitor
6. Install XMODEM in new CF disk
7. XMODEM UNARJ.COM to decompress subsequent files
8. XMODEM CP/M 2.2 system files
9. XMODEM CP/M 3 system files
10. XMODEM ZORK1,2,3
11. XMODEM HiTech C 3.09
12. Decompress CPM 3 system files into drive A:
13. Decompress CPM 2.2 system files into drive B:
14. Decompress HiTech C files into drive C:
15. Decompress ZORK1,2,3 into drive D:
It takes about 7 minutes to do all above, but they are all done automatically. Here is a YouTube video of the entire process. https://youtu.be/0L9N5JCj-V8

While this macro works well, it can use some improvements:
1. A way to slow down the 'send' command so there is small delay between each character sent. Right now I send 5 characters, wait 100mS, send 5 more, wait, etc. It works, but it is ugly.
2. A way to set the default directory for MACRO. Right now I specify the filepath to “c:\teraterm\newcf”; I like to have more flexibility where files are stored.

Software
All files required to create a new CF disk

