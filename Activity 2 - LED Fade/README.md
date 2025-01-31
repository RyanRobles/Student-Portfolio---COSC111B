# Laboratory Activity #2

## Objectives: 
1. Discuss analog signals and its implementation in a Arduino circuit.
2. Understand analog to digital signal conversion using the map() function.
- The objective of this project is to create a running light effect using multiple LEDs. The LEDs will gradually increase in brightness and then turn off one by one, creating a smooth transition effect.

## Instructions  
Building on the first activity, implement the same logic with the following conditions:  

- Use **pins 8 to 12** for the LEDs.  
- Create a **running light effect** from pin **12 to 8**, turning LEDs on one by one with a **1-second delay**, then turning them off sequentially.  
- Use `analogWrite()` to control the brightness of the LEDs.  
- Implement the logic using a **while() loop** and an **array** to set the pin modes.  

## Description  
This project controls multiple LEDs connected to an Arduino, creating a **smooth transition effect** by gradually increasing their brightness and turning them off sequentially. This demonstrates how to work with **analog signals** and the `map()` function to adjust LED brightness dynamically.  

## To Run:   
1. **Connect the LEDs** to the specified pins on your Arduino.  
2. **Upload the code** to your Arduino.  
