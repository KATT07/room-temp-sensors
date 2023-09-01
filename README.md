# room-temp-sensors
This is a modification of the original code to replace pressure with heatindex calculations
+ Added support for gas sensor MQ135

Original code by : https://randomnerdtutorials.com/esp8266-nodemcu-mqtt-publish-bme280-arduino/



# Prerequisites

You need to setup a MQTT Broker on the same network as your esp8266

# How to setup
Make sure u have Git installed then run
"git clone https://github.com/KATT07/room-temp-sensors"
Then open the file in Arduino IDE
goto Sketch > Include Library > Add . ZIP library and select the libraries you’ve just downloaded.
For BME280 need to add the Adafruit BME280 library with dependencies in arduino software
For MQ135 need to add the MQ135 library in same folder as the code.ino : https://github.com/GeorgK/MQ135


# Hardware:
Connect BME280:                                                                                                                                                                                                                            
Vcc -> Vcc                                                                                                                                                                                                                                   
Gnd -> Gnd                                                                                                                                                                                                                               
SCL(Clock) -> D1 pin                                                                                                                                                                                                                          
SDA(Data) -> D2 pin                                                                                                                                                                                                                           

Connect MQ135:                                                                                                                                                                                                                            
Vcc -> Vcc                                                                                                                                                                                                                             
Gnd -> Gnd                                                                                                                                                                                                                             
AO -> A0 pin                                                                                                                                                                                                                             

# Software:
Replace the XXX with corresponding values for Software
