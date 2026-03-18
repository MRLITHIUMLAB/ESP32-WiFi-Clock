# ESP32 WiFi Desktop Clock ⏰

A simple WiFi-based clock using ESP32 that shows real-time on OLED and 16x2 LCD.

## 🚀 Features

- Real-time clock using internet (NTP)
- 12-hour format with AM/PM
- Day (Mon, Tue, Wed)
- Date display
- Works on OLED and LCD
- No RTC module required

---

## 🧰 Components

- ESP32
- OLED Display (0.9" I2C)
- 16x2 LCD with I2C
- Jumper wires

---

## 🔌 Wiring

### OLED

- VCC → 3.3V  
- GND → GND  
- SDA → GPIO 21  
- SCL → GPIO 22  

### LCD

- VCC → 5V  
- GND → GND  
- SDA → GPIO 21  
- SCL → GPIO 22  

---

## 📚 Libraries

Install from Arduino Library Manager:

- Adafruit SSD1306  
- Adafruit GFX  
- LiquidCrystal I2C  

---

## ⚙ Setup
1.use 2.4 ghz wifi.
2. Enter your WiFi credentials:
const char* ssid = "YOUR_WIFI";
const char* password = "YOUR_PASSWORD";

##🌍 Timezone
India = GMT +5:30
Convert to seconds:
5 × 3600 = 18000
30 × 60 = 1800
Total = 19800

code :
const long gmtOffset_sec = 19800;

