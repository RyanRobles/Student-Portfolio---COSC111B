# Laboratory Activity #1


## Objectives  
This project creates a system that controls LEDs in a specific order, turning them on and off one by one. Users can choose to activate either odd-numbered or even-numbered LEDs separately.  

## Description  
This project uses an Arduino to control multiple LEDs, making them light up and turn off in sequence with a short delay. The process repeats continuously.  

## Components  
- **LED Pins (`ledPins[]`)**: Stores the pin numbers connected to the LEDs.  
- **Number of LEDs (`numLeds`)**: Specifies the total number of LEDs.  
- **Setup**: Configures LED pins as outputs.  
- **Loop**: Controls the order in which LEDs turn on and off.  

## Instructions  

1. **Connect the LEDs**: Attach the LEDs to the correct pins on the Arduino.  
2. **Upload the Code**: Transfer the program to the Arduino.  
3. **Run the Program**: The LEDs will turn on and off in sequence with a one-second delay.  
4. To light up **only odd-numbered LEDs**, update the loop to activate LEDs at odd positions.  
5. To light up **only even-numbered LEDs**, adjust the loop to activate LEDs at even positions.  
