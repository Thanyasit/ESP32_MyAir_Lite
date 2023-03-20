<h1>MyAir Lite</h1>
<h2>Description</h2>
This is a simple air quality monitor that measures the concentration of PM2.5 particles in the air using an ESP32 and an SPS30 sensor. The device calculates the Air Quality Index (AQI) based on the concentration of PM2.5 particles in the air and sends the data via Bluetooth. The device also features a single LED light that changes color based on the air quality.
<h2>Getting Started</h2>
<h3>Prerequisites</h3>
Arduino IDE
ESP32 board libraries for Arduino IDE
FastLED library
sensirion_uart library
sps30 library
<h3>Installation</h3>
Clone this repository.
Connect the ESP32 to your computer using a USB cable.
Open the Air_Quality_Monitor.ino file in Arduino IDE.
Go to Tools > Board and select your ESP32 board.
Install the required libraries using Sketch > Include Libraries > Manage Libraries.
Upload the code to your ESP32 by clicking Sketch > Upload.
<h2>Usage</h2>
Power on the ESP32.
The LED light will turn on for 0.5 seconds and then turn off.
The device will start measuring the concentration of PM2.5 particles in the air and display the value in the Arduino Serial Monitor.
The device will then calculate the AQI based on the PM2.5 concentration and display the AQI level in the Arduino Serial Monitor.
The device will send the AQI level via Bluetooth to a device named "MyAir_Case".
The LED light will change color based on the AQI level:
Green: AQI level 0-50
Yellow: AQI level 51-100
Orange: AQI level 101-150
Red: AQI level 151-200
Purple: AQI level 201-300
Brown: AQI level 301-500
Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
<h2>License</h2>
This project is licensed under the MIT License - see the LICENSE file for details3
