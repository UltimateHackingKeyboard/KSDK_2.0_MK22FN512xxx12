Overview
========

The SDSPI example shows how to use SDSPI driver to initializes SD card and read/write data blocks 
of SD card. It calls read/write APIs of the driver to read/write single and multiple data blocks
of SD card forever until encounters some error to result in the read data content is different the 
original data content written to the card.

The example only uses the polling transaction API of SPI driver to send/receive data 
over SPI bus. More detail transaction API of SPI driver can refer to the SPI driver and SPI example.


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
- TWR-MEM board
- Personal Computer

Board settings
==============
The SDCARD Polling example is configured to use SPI1 with PTB10, PTB11, PTB16, PTB17 pins
and use PTE6 pin as card detection pin. SD card should be inserted in the card slot of TWR-MEM
board. The pin 1-2 of J12 on TWR-MEM board must be connected and pin 3-4 of J12 on TWR-MEM board
must be removed.

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
When the example runs successfully,you can see the similar information from the terminal as below:

SD card over SPI example start.

Please insert the SD card
Detected SD card inserted.

Read/write SD card continuously until encounters error.

Write/read one data block......
Compare the read/write content......
The read/write content is consistent.

Write/read multiple data blocks......
Compare the read/write content......
The read/write content is consistent.

Input 'q' to quit read/write process.
Input other char to read/write data blocks again.

Customization options
=====================


