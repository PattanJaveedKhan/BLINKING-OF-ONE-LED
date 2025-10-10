# Blinking LED 💡

This is a simple project where I made an LED blink using Arduino.  
It helps to understand how to use digital pins for output and how the delay function works.

---

## Components Used
- ESP32
- LED
- 220Ω Resistor
- Breadboard
- Jumper Wires

---

## Working
The Arduino turns the LED ON and OFF repeatedly with a small delay in between.  
When the output pin is set to HIGH, the LED turns ON, and when it is LOW, the LED turns OFF.

---
![video](https://github.com/user-attachments/assets/8c8bef15-3ad5-4207-b66e-bbfa1183cf91)

## Code
```cpp
int led = 13;   // LED connected to pin 13

void setup() {
  pinMode(led, OUTPUT);
}

void loop() {
  digitalWrite(led, HIGH);  // Turn LED ON
  delay(1000);              // Wait for 1 second
  digi

