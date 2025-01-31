# Laboratory Activity #4

## Objectives:
- Understand and implement Arduino Serial Connection
- Utilize and familiarize students on different basic Serial connection functions
- Create a simple circuit that can be controlled using Serial connection

## Instructions:
- Using the diagram and code base used for Laboratory Activity 3, fulfill the following:
1. Choose one (1) sensor to be used in this activity
2. If using thermistor, set the temperature threshold to 50 Celsius. If using photoresistor, set the brightness threshold to 220.
3. If the threshold is met, blink the LED in pin 13 (delay = 100) AND SHOULD continue to blinking even after the sensor reading is below threshold.
4. If the word "stop" is entered in the Serial Monitor, the blinking should stop. The word should be case insensitive (can enter stop in different cases)

## How to Run  

1. **Connect the selected sensor** (thermistor or photoresistor) and **LED** to the correct pins on the Arduino.  
2. **Upload the code** to your Arduino board.  
3. **Open the Serial Monitor** in the Arduino IDE.  
4. **Trigger the threshold condition** by increasing temperature (for a thermistor) or brightness (for a photoresistor).  
5. **Observe the LED blinking continuously** once the threshold is met.  
6. **Type `"stop"` in the Serial Monitor** to turn off the LED blinking.  
