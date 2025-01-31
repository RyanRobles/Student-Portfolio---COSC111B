# Laboratory Activity #6

## Objectives:
- Develop a system that detects button presses using an Arduino and transmits the button state to a Python script.
- Implement API-based control, where the Python script triggers an HTTP request based on the button press.
- Establish a wireless connection (Wi-Fi or hotspot) between devices for remote communication.

## Components: 
Hardware:
- Arduino board
- USB cable for connection

Software:
- Arduino IDE
- Python (version 3.x)
- Required Libraries : pip install pyserial requests fastapi[standard]


## Description:
- This project focuses on button press detection using an Arduino, which then communicates the button state to a Python script via serial communication. The script subsequently triggers an API request to another device connected via Wi-Fi or a hotspot. This second device has its own Arduino and LED setup, which responds to the received API commands.

## Steps to Implement

1. **Build the circuit** according to the diagram in `A6-Diagram.png`.
2. **Upload the Arduino code** (`.ino` file) to the Arduino using the Arduino IDE, making sure to select the correct serial port.
3. **Update the Python script** with your local IP address so it can properly communicate with the Arduino via the serial connection.
4. **Set up FastAPI** to control the LED remotely by changing its state when a button is pressed.
5. **Use the `requests` library** to send HTTP requests that trigger the LED changes when the button is pressed.

## Running the Server:
- To start the FastAPI server, execute:fastapi dev <name_of_file>.py

## Testing the API via Command Line:
- Turn LED On: curl -X POST http://127.0.0.1:8000/led/on
- Turn LED Off: curl -X POST http://127.0.0.1:8000/led/off

## Key Concepts in the Python Code

- **Button Press Detection**: The Arduino continuously checks the button's state and sends updates through the serial connection.
- **Serial Communication**: The Python script listens for serial input from the Arduino.
- **API Call Trigger**: When the button is pressed, the script sends an HTTP request to control the LED on a second Arduino.
- **Network Communication**: The system uses Wi-Fi or a hotspot to enable communication between the two devices.

---

## Additional Note

- This activity builds on **Laboratory Activity 5**, where the remote LED system is controlled by the button system on this Arduino.
