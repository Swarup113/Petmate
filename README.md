# PetMate - Smart Pet Feeder
PetMate is an IoT-based automated pet feeding system designed to provide convenience and peace of mind to pet owners. By leveraging the power of the ESP8266 microcontroller and web technology, PetMate allows users to feed their pets remotely or on a schedule, ensuring pets are never left hungry even when their owners are away.

## About the Project
In the modern era of automation, PetMate aims to simplify pet care. It is an automatic feeding machine controlled via a custom web interface. The system uses a NodeMCU (ESP8266) as the central processing unit, interfaced with a servomotor to control the dispensing of food. When activated, the servo rotates to open a food portal, allowing food to drop into a bowl, and then returns to its resting position.

## Motivation
Pet ownership is a rewarding but time-consuming responsibility. A common issue faced by owners is the inability to feed their pets on time due to work, travel, or social commitments. PetMate eliminates this worry by acting as a remote surrogate, ensuring pets receive their meals punctually. It bridges the gap between a busy lifestyle and responsible pet parenting.

## Features
- Web-Based Control: Control the feeder from anywhere via a dedicated HTML webpage.
- Two Feeding Modes:
- Automatic: A pre-configured routine to dispense food without user intervention.
- Manual: Direct control via buttons or a slider on the web interface.
- Precise Dispensing: Adjust rotation speed and angles to control the amount of food dispensed.
- Cost-Efficient: Designed to be affordable and easy to use for non-technical users.

## Hardware Requirements
- NodeMCU (ESP8266): The microcontroller acting as the "heart" of the system.
- Servo Motor: Used to physically control the food container's opening/closing mechanism.
- Connecting Wires: Jumper wires for circuit connections.
- USB Cable: For power and communication with the PC.
- Food Container & Bowl: A storage unit for pet food and a bowl for serving.

## Circuit Diagram & Connections
The circuit is designed using Fritzing software. The connections are as follows:
- Servo Motor Pin
- NodeMCU Pin
- Signal (Orange/White)	D1
- VCC (Red)	3.3V
- GND (Brown/Black)	GND

## Software Implementation
1. Arduino IDE
The logic for the microcontroller was developed in the Arduino IDE.
Library Used: Servo Library to interface with the motor.
Code Logic: Defines specific angles for the servo to rotate (opening the portal) and return to the resting point (closing the portal).

2. Web Interface (PetMate)
A webpage was created using HTML to serve as the user interface.
The system connects to a Wi-Fi network.
The NodeMCU acts as a web server (or communicates via the PC server bridge as implemented).
The interface provides buttons and sliders to trigger the servo motor actions remotely.

## Feed Your Pet:
Use the Automatic button for a pre-set feeding cycle.
Use the Manual slider/buttons to dispense a specific amount of food instantly.

Created with love for pets and their owners.
