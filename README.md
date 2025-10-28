# Anti-Theft-Alert-System-using-Tilt-Sensor

### Name: Mathan Kailash S
### Reg No: 212223060156
### Slot: 4X4-5

## Aim:
To measure the tilt Sensor using SW200D with Arduino UNO Board/ESP-32 using Tinker CAD.

## Hardware / Software Tools required:

#### PC/ Laptop with Internet connection
#### Tinker CAD tool (Online)
#### Arduino UNO Board/ESP-32
#### Tilt sensor(SW200D)

## Circuit Diagram:
 ![WhatsApp Image 2025-10-28 at 18 53 40_35360d3b](https://github.com/user-attachments/assets/6be42cad-0d70-4da1-a091-fa9655061703)

## Theory :
 The Arduino Uno is powered by the ATmega328P, an 8-bit microcontroller that runs at 16 MHz. It has 32 KB of flash memory, 2 KB of SRAM, and 1 KB of EEPROM. The board has 14 digital I/O pins (of which 6 can be used as PWM outputs) and 6 analog input pins. These pins allow the board to interface with various sensors, actuators, and other devices.The Arduino Uno can be powered via a USB connection or an external power supply. The board has a built-in voltage regulator to manage power from 7 to 12 volts.
The board is programmable using the Arduino IDE (Integrated Development Environment), which supports a simplified version of C/C++. The code, known as a "sketch," is uploaded to the board via a USB connection. The Uno has a USB-B port, which is used for communication with a computer. The USB connection also powers the board when connected. The board includes a reset button that restarts the microcontroller, useful during programming and troubleshooting. The In-Circuit Serial Programming (ICSP) header allows for low-level programming of the microcontroller or firmware updates. The Uno has a built-in LED on pin 13, commonly used for simple tests and debugging.


## Procedure:

Step 1: Set Up the Tinkercad Environment
•	Log in to Tinkercad: Open Tinkercad in your web browser and log in to your account.
•	Create a New Circuit: In the Tinkercad dashboard, click on "Circuits" and then select "Create New Circuit."
Step 2: Add Components to the Circuit
•	Arduino Uno: Drag an Arduino Uno board from the components panel onto the workspace.
•	SW200D Sensor: Search for the SW200D sensor in the components panel and drag it into the workspace.
•	Breadboard: Drag a small breadboard to the workspace to help with wiring connections.
•	Resistor (Optional): A resistor may not be necessary for this simple setup, but you can include it for more accurate readings.
•	Wires: Use wires to connect the components.

Step 3: Connect the Tilt Sensor (SW-200D) to Arduino:
•	SW200D Vout (Middle Pin) to Arduino Digital Pin (e.g., D2): Use a wire to connect the middle pin (Vout) of the tilt sensor to a digital input pin on the Arduino.
•	SW200D GND (One Side Pin) to Breadboard GND Rail: Connect one side pin of the tilt sensor to the ground rail of the breadboard.
•	SW200D VCC (Other Side Pin) to Breadboard 5V Rail: Connect the other side pin of the tilt sensor to the 5V rail of the breadboard.
Step 4: Write the Arduino Code
•	Code Editor: Click on the "Code" button at the top of the Tinkercad workspace to open the code editor.
•	Set the Coding Mode: Ensure the editor is in "Text" mode to write your code in C/C++.
•	Enter the Code: Write the following code from the SW200D sensor:
Step 5: Simulate the Circuit
•	Start Simulation: Click the "Start Simulation" button at the top of the workspace to run the circuit and code.
•	Monitor Output: Open the serial monitor by clicking the "Serial Monitor" button 
Step 6: Troubleshoot and Refine
•	Check Connections: Ensure that all connections are made correctly on the breadboard and the Arduino.
•	Adjust Code: If needed, tweak the code to improve accuracy or change the format of the output.
Step 7: Save Your Work
•	Stop Simulation: Click "Stop Simulation" to end the simulation.
•	Save the Circuit: Click "Save" to keep your circuit design and code for future use.

## Code:
```
int ledPin=13;
int inPin=7;
void setup()
{
 Serial.begin(9600);
  pinMode(ledPin,OUTPUT);
  pinMode(inPin,INPUT);
}
void loop()
{
  int val=digitalRead(inPin);
  if(val==0)
  {
    digitalWrite(ledPin,HIGH);
  }
  else
  {
    digitalWrite(ledPin,LOW);
  }
}
```



## Output:
![WhatsApp Image 2025-10-28 at 18 53 18_0553e39a](https://github.com/user-attachments/assets/0b50afd7-52ed-4914-a4f8-76ab77a71880)

 ## Result:
 Thus measure the Tilt Sensor using SW200D with Arduino UNO Board/ESP-32 using Tinker CAD has been Verified Successfully.

