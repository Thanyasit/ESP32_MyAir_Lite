<h1>ESP32 MyAir Lite</h1>
<h2>Description</h2>
This is a arduino program for MyAir Lite that uses the Adafruit BME280 and Plantower PMS5003 sensors to measure temperature, humidity, and air quality (PM2.5) and display the result on LED lights. The program also sends the data over Bluetooth using the BluetoothSerial library.<br>
<b>2020</b>
<h2>Prerequisites</h2>
Before using this program, make sure you have the following libraries installed:<br><br>  

- Wire.h - included with Arduino IDE<br> 
- SPI.h - included with Arduino IDE<br> 
- Adafruit_Sensor.h - install from the Arduino Library Manager<br> 
- Adafruit_BME280.h - install from the Arduino Library Manager<br> 
- PMS.h - install from the Arduino Library Manager<br> 
- BluetoothSerial.h - install from the Arduino Library Manager<br> 
<h2>Set up</h2>
1.Connect the BME280 sensor and PMS5003 sensor to the appropriate pins on the MyAir Lite board.<br> 
2.Upload the program to the MyAir Lite board using the Arduino IDE.<br> 
3.Pair your Bluetooth device with the MyAir Lite board. The device name is "MyAir_Lite".<br> 
4.Turn on the MyAir Lite board.
<h2>Usage</h2>
The MyAir Lite board will display the air quality level on the LED lights. If the air quality is good (PM2.5 <= 10), the first LED will turn on. If the air quality is moderate (10 < PM2.5 <= 20), the first two LEDs will turn on. If the air quality is unhealthy (20 < PM2.5 <= 37), the first three LEDs will turn on. If the air quality is very unhealthy (37 < PM2.5 <= 50), the first four LEDs will turn on. If the air quality is hazardous (50 < PM2.5 <= 90), the first five LEDs will turn on. If the air quality is very hazardous (PM2.5 > 90), all six LEDs will turn on.<br> <br> 

The program will also send the temperature, humidity, and PM2.5 data over Bluetooth every three seconds.

To put the MyAir Lite board into deep sleep mode, press the reset button on the board or connect the <b>'EN'</b> pin to the <b>'RST'</b>  pin using a jumper wire. The board will wake up every three minutes to take new measurements.

<h3>PCB Design</h3>

<h3>Basic Appication</h3>

<h3>Product</h3>

<h2>License</h2>
This program is licensed under the MIT License. See the LICENSE file for details.
