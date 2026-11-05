Arduino-Based Two-Channel Relay Control System

📌 Project Overview

This project demonstrates an Arduino-based two-channel relay control system. It uses an Arduino UNO to control two relay channels connected to digital pins 3 and 4.

Both relays automatically turn ON and OFF with a time delay of 2 seconds. This project demonstrates basic relay interfacing and digital output control in embedded systems.

🛠️ Components Required

- Arduino UNO
- Two-Channel Relay Module
- Jumper Wires
- USB Cable

🔌 Circuit Connections

Relay Module| Arduino UNO
IN1| Digital Pin 3
IN2| Digital Pin 4
VCC| 5V
GND| GND

⚙️ Working Principle

1. Arduino initializes pins 3 and 4 as OUTPUT.
2. Both relay channels receive a LOW signal.
3. Both relays turn ON.
4. The system waits for 2 seconds.
5. Both relay channels receive a HIGH signal.
6. Both relays turn OFF.
7. This process repeats continuously.

💻 Arduino Code

int relay1 = 3;
int relay2 = 4;

void setup() {
  pinMode(relay1, OUTPUT);
  pinMode(relay2, OUTPUT);
}

void loop() {
  digitalWrite(relay1, LOW);
  digitalWrite(relay2, LOW);
  delay(2000);

  digitalWrite(relay1, HIGH);
  digitalWrite(relay2, HIGH);
  delay(2000);
}

📚 Concepts Learned

- Digital Input and Output
- Relay Module Interfacing
- Arduino GPIO Control
- HIGH and LOW Signals
- Time Delay using "delay()"
- Embedded Systems Basics

🎯 Applications

- Home Automation
- Electrical Load Switching
- Water Pump Control
- Appliance Control

🏁 Conclusion

This project provides practical experience in interfacing a two-channel relay module with Arduino. It demonstrates automatic ON/OFF switching and helps develop fundamental embedded systems skills.

Note: This code assumes an active-LOW relay module (LOW = ON, HIGH = OFF).
