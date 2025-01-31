# Laboratory Activity 3

## Objectives:
- This project aims to implement a fire detection system using an Arduino. It utilizes a temperature sensor and a photoresistor to detect high temperatures and brightness levels, triggering an LED warning signal if a fire is detected.

## Instructions  

**1. Wiring the Sensors**: Connect the temperature sensor, photoresistor and LED to the designated pins on the microcontroller.  
**2. Uploading the Code**: Transfer the program to the Arduino board.  
**3. Executing the System**: The system will continuously monitor temperature and brightness.  
**To Adjust Sensitivity**: Change the `Tempmax_Treshold` and `Brightnessmax_Treshold` values for different detection levels.  
**Customization**: Modify the LED blinking pattern for different alert signals.  

## Components  
- **Temperature Sensor (`Temp_Sensor_Pin`)**: Reads temperature values.  
- **Photoresistor (`Photo_Sensor_Pin`)**: Detects ambient brightness.  
- **LED Indicator (`LED_PIN`)**: Flashes when fire conditions are met.  
- **Temperature Threshold (`Tempmax_Treshold`)**: Maximum allowable temperature before fire detection triggers.  
- **Brightness Threshold (`Brightnessmax_Treshold`)**: Maximum brightness level before fire detection triggers.  
- **Beta Value (`BetaValue`)**: Used for thermistor calculations.  
- **Series Resistance (`Series_Resistance`)**: Part of the resistance network for temperature measurement.  

## How to Use  
1. **Connect the sensors** (temperature sensor and photoresistor) to the designated pins on the microcontroller.  
2. **Upload the code** to the microcontroller.  
