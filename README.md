# Designing and Developing Device Drivers

## Prelims  
https://www.youtube.com/results?search_query=craig+duffy+olimex - handy seminars, also can be found on Blackboard.  
Create project directory 'dd' (where this file lives).

#### Available Sheets  
###### Year 2 Worksheets
 - Worksheet 1: OpenOCD
 - Worksheet 2: ARM Cortex M3 intro and tools
 - Worksheet 3: Clocks, GPIO, Makefile
 - Worksheet 4: USART, RS232
 - Worksheet 5: Debugging, Logic Analyser  
 - Worksheet 6: Building and Configuring Libraries
 - Worksheet 7: Programming Interrupts and Timers
 - Worksheet 8: FreeRTOS  

###### Year 3 Worksheets [2 Required]
 - Worksheet 9: USB  
 - Worksheet 10: TCP/IP
 - Worksheet 11: Cube, SPI, SD Cards and FATFS

#### Recommended Start

 - Worksheet 6 (building libraries)
 - Worksheet 8 (FreeRTOS)  
 _USB sheet not recommended unless very interested_

## Worksheet 1
This sheet is mostly about making sure we can serial to the Olimex Board.  

 - make sure JTAG is connected to board and plug into USB. (a red LED should be on on the board)
 - plus serial into serial on board, and USB via an adapter to PC

###### Running OpenOCD

Open a new terminal in the project directory, and create a new file call openocd.cfg - his is to save all the settings needed for talking to the board - then open openocd.
```
touch openocd.cfg  

openocd -f openocd.cfg  
```


## Worksheet 6  
Completing this as the first (old worksheets not on new system), so may repeat some steps from previous.  

Start by grabbing the .tgz file from Blackboard, and moving it into the project directory/project_files
