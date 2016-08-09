Overview
========
This example show application of FatFs with SD card controled over SPI interface. It mounts a file
system based on a SD card then does "creat directory/read directory/create file/write file/read file"
operation.

Toolchain supported
===================
- IAR embedded Workbench 7.50.1
- Keil MDK 5.17
- GCC ARM Embedded 2015-4.9-q3
- Kinetis Development Studio IDE 3.0.0
- Atollic TrueSTUDIO 5.4.0

Hardware requirements
=====================
- Mini/micro USB cable
- TWR-K22F120M board
- Personal Computer

Board settings
==============
The SDCARD Polling example is configured to use SPI1 with PTB10, PTB11, PTB16, PTB17 pins
and use PTC5 pin as card detection pin.

Prepare the Demo
================
1. Connect a USB cable between the PC host and the OpenSDA USB on the board.
2. Open a serial terminal on PC for OpenSDA serial device with these settings:
   - 115200 baud rate
   - 8 data bits
   - No parity
   - One stop bit
   - No flow control
3. Download the program to the target board.
4. Either press the reset button on your board or launch the debugger in your IDE to begin running
   the example.

Running the demo
================
When the example runs successfully,you can see the similar information from the terminal as below.
~~~~~~~~~~~~~~~~~~~~~
FATFS example to demonstrate how to use FATFS with SD card over SPI.
Please inserts a card into board.
Detected SD card inserted.
Make file system......The time may be long if the card capacity is big.
Create directory......
Create a file in that directory......
List the file in that directory......
General file : F_1.DAT.
Directory file : DIR_2.
Write/read file until encounters error......
Write to above created file.
Read from above created file.
Compare the read/write content......
The read/write content is consistent.
Input 'q' to quit read/write.
Input other char to read/write file again.
~~~~~~~~~~~~~~~~~~~~~

Customization options
=====================


