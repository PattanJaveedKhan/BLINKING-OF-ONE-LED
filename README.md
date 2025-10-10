# Blinking LED 💡

This is a simple project where I made an LED blink using esp32 
It helps to understand how to use digital pins for output and how the delay function works.

---

 Components Used
- ESP32
- LED
- 220Ω Resistor
- Breadboard
- Jumper Wires

---

 Working
The Arduino turns the LED ON and OFF repeatedly with a small delay in between.  
When the output pin is set to HIGH, the LED turns ON, and when it is LOW, the LED turns OFF.

---

https://github.com/user-attachments/assets/11899e7c-e2f8-4712-9b25-2237eeef4dc8

code
```cpp
int led = 13;   // LED connected to pin 13

void setup() {
  pinMode(led, OUTPUT);
}

void loop() {
  digitalWrite(led, HIGH); 
  delay(1000);              
  digitalWrite(led, LOW);   
  delay(1000);              
}
