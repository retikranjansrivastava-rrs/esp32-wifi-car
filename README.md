# esp32-wifi-car
 Wi-Fi controlled car robot using ESP32 and Arduino. Move forward, backward, left, right, and stop, with adjustable motor speed via a simple web interface. Perfect for learning ESP32, web-controlled robotics, and PWM motor control. Includes circuit diagram and setup instructions.
# ESP32 Wi-Fi Car Robot

![Wi-Fi Car](images/wifi_car_photo.png)

A Wi-Fi controlled car robot using the ESP32 microcontroller and Arduino IDE. Control the car's movements and motor speed from any device through a web browser.

---

## Features

- Move Forward, Backward, Left, Right, and Stop
- Adjustable motor speed via web slider
- Simple web interface for easy control
- Uses ESP32's PWM for precise motor speed control

---

## Circuit Diagram

![Circuit Diagram](images/wifi_car_circuit.png)

**Motor Pins (ESP32):**

| Motor | Pin 1 | Pin 2 | Enable (PWM) |
|-------|-------|-------|--------------|
| Motor 1 | 27 | 26 | 14 |
| Motor 2 | 33 | 25 | 32 |

---

## Hardware Required

- ESP32 Development Board  
- 2x DC Motors  
- Motor Driver (L298N or similar)  
- Jumper wires  
- 5V Power supply  

---

## Software Required

- Arduino IDE  
- ESP32 Board Package  
- Libraries: WiFi.h, WebServer.h  

---

## Setup Instructions

1. Connect your ESP32 to your computer.  
2. Open `esp32_wifi_car.ino` in Arduino IDE.  
3. Replace your Wi-Fi credentials:  

```cpp
const char* ssid     = "YOUR_SSID";
const char* password = "YOUR_PASSWORD";
