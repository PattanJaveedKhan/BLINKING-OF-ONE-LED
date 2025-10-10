# Blinking LED 💡

This project demonstrates how to make an LED blink at regular intervals using a microcontroller (Arduino).  
It’s one of the simplest and most important beginner projects to understand how digital output and timing work in embedded systems.

---

## 🔧 Components Used
- Arduino Uno (or any compatible microcontroller)
- LED
- Resistor (220Ω)
- Jumper wires
- Breadboard

---

## ⚙️ Working Principle
The Arduino sends a HIGH signal to the GPIO pin to turn the LED ON and a LOW signal to turn it OFF.  
By adding a small delay between these operations, the LED appears to blink continuously.

---

## 🧠 Learning Outcome
- Basic GPIO output control  
- Understanding of digital HIGH/LOW signals  
- Using the `digitalWrite()` and `delay()` functions in Arduino  
- Setting up simple electronic circuits on a breadboard  

---

## 📸 Demo
![Blinking LED](images/blink-demo.jpg)

---

## 📽️ Video
[▶ Watch demo video](https://youtu.be/YOUR_VIDEO_LINK)

---

## 📁 Code
See `code/blink.ino`

Example Arduino code:
```cpp
int ledPin = 13; // Built-in LED pin on most Arduino boards

void setup() {
  pinMode(ledPin, OUTPUT); // Set the pin as output
}

void loop() {
  digitalWrite(ledPin, HIGH); // Turn LED ON
  delay(1000);                // Wait 1 second
  digitalWrite(ledPin, LOW);  // Turn LED OFF
  delay(1000);                // Wait 1 second
}

