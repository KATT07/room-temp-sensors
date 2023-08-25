# room-temp-sensors
This is a modification of the original code to replace pressure with heatindex calculations
+ Added support for gas sensor MQ135

Original code by : https://randomnerdtutorials.com/esp8266-nodemcu-mqtt-publish-bme280-arduino/



# Prerequisites

follow the original code for installing mqtt libraries

Installing the Async MQTT Client Library : https://github.com/marvinroger/async-mqtt-client/archive/master.zip
Rename your zip file from async-mqtt-client-master to async_mqtt_client
and then goto Sketch > Include Library > Add . ZIP library and select the library you’ve just downloaded.

Installing ESPAsync TCP Client Library : https://github.com/me-no-dev/ESPAsyncTCP
Rename your folder from ESPAsyncTCP-master to ESPAsyncTCP
and then goto Sketch > Include Library > Add . ZIP library and select the library you’ve just downloaded.

for BME280 need to add the Adafruit BME280 library with dependencies in arduino software

for MQ135 need to add the MQ135 library in same folder as the code.ino : https://github.com/GeorgK/MQ135

And also need to have a mqtt broker setup on a pc on the same network as the mqtt publisher

# How to setup
# for Hardware:
Connect BME280:
Vcc -> Vcc
Gnd -> Gnd
SCL(Clock) -> D1 pin
SDA(Data) -> D2 pin 

Connect MQ135:
Vcc -> Vcc
Gnd -> Gnd
AO -> A0 pin

# for Software:
replace the XXX with corresponding values for software
