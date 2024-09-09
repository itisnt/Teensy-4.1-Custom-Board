# Teensy-4.1-Custom-Board

Simple Board for a Teensy 4.1 with Ethernet, 2 x I2C ports and a port with RX1/TX1 

You need (beside the PCB...):
- A Teensy 4.1 board https://www.pjrc.com/store/teensy41.html
- The Ethernet kit https://www.pjrc.com/store/ethernet_kit.html (you need the MagJack, the capcitor and mybe the headers)
- If you use I2C, you should add the two SMD 0603 resistors (1 - 10kohm). There are internal pull-ups in the Teensy, but they are quite weak

![Board in use as a sensor board](Board01.png)

![3D view from KiCad](Board02.png)

## Some remarks:
- It's my first KiCad board, so a lot of things will be wrong (i assume...)
- Since i use https://aisler.com to produce the PCB and Aisler allows to simply upload the _pcb file from KiCad, all the Gerber stuff is untested. So don't simply upload the gerber files. Setup KiCad 8 and create your own gerber files
- KiCad 8.0.5 was used
- Since i didn't find the right MagJack in KiCad i had to edit the Symbol for one of the MagJack available in KiCad. What i did was reordering R1-R8. Thats why there is a custom lib. And also you need the Teensy Lib which i've found somewhere in the internet. 
- I do not sell any PCB's

## Ideas for the future:
- Make more pins available (SPI foremost)
- Center the top I2C header so that the Adafruit 4-Segment Display is more in the middle of the board
- Maybe add an FRAM (SPI based)