# 24-Second Countdown Timer (TTL Logic)  
## Overview  
This project is a 24-second countdown timer implemented using classic TTL logic ICs. The design is captured and laid out in KiCad and drives common-cathode 7-segment displays through BCD decoding logic. The system includes user control via a slide switch (enable) and a tactile push button (load data).  
The project demonstrates the practical use of up/down counters, BCD-to-7-segment decoding, and basic control logic.  

## Functional Description  
### Counter Operation  
The 74192 counter is configured to perform a count-down operation.  
The timer starts from a preset value corresponding to 24 seconds.  
Each clock pulse decrements the count by one.  
### Display Logic  
The 4-bit BCD output from the 74192 feeds directly into the 7448.  
The 7448 decodes the BCD value and drives the common-cathode 7-segment display.  
Segment current limiting is handled by external resistors.  

## Controls  
### Slide Switch (Enable)  
ON: Enables the countdown operation  
OFF: Pauses or disables the counter  
### Tact Switch (load data)  
Used to manually load the data corresponding to 24 decimal digit. 
