# Laboratory Activity #5

## Objectives:
- Learn how to use **Arduino Serial Communication**.
- Use **Python** to manage serial connections.
- Create a system where you can control an **Arduino circuit** using **Python** and **FastAPI** via HTTP requests.

## Description:
In this project, you’ll set up a **serial communication** interface between an **Arduino board** and a **FastAPI backend**. This will allow you to control an **LED** remotely by sending HTTP requests to the FastAPI server, which will communicate with the Arduino to turn the LED on or off.

## Components 
### Hardware:
- **Arduino board**
- **USB cable** to connect the Arduino to your computer

### Software:
- **Arduino IDE** to upload code to the Arduino
- **Python (version 3.x)** installed on your computer

## Implementation Steps:
- Set up the circuit according to the diagram in `A5-Diagram.png`.
- Upload the Arduino code using the **Arduino IDE**, ensuring the correct serial port is selected.
- Create a **Python script** to send commands to the Arduino through the serial port.
- Use **FastAPI** to create an API that controls the Arduino.

## Running the Server:
- To start the FastAPI server, use the following command: fastapi dev <name_of_file>.py

## Testing the API via Command Line:
- Turn LED On: curl -X POST http://127.0.0.1:8000/led/on
- Turn LED off:curl -X POST http://127.0.0.1:8000/led/off
## Key Concepts in the Python Code:
- **Serial Initialization**: Connects to the Arduino using **COM5** and a **9600 baud rate**.
- **Delay (2 seconds)**: Gives the Arduino enough time to reset and initialize properly.
- **Write Commands**: Sends `"1"` to turn the LED on and `"0"` to turn it off through the serial interface.

## Additional Notes:
- This activity can be expanded in **Laboratory Activity 6**, where a second Arduino setup will be used to control the LED system remotely.
- This project demonstrates how **embedded systems** can be integrated with **web technologies**, laying the groundwork for **IoT applications**.
