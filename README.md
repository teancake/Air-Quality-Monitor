# Air-Quality-Monitor
Schematic and PCB design of an air quality monitor.

### Description ###
This WiFi switch module utilises the [ESP-12E/F adaptor](https://github.com/teancake/ESP8266-ESP12-Adaptor "ESP-12E/F Adaptor").
### Programs ###
There are two ways of programming this piece of hardware:
1. Program both the AVR chip on the Arduino board and the ESP8266 chip on the ESP-12E/F board.
2. Program only the AVR chip on the Arduino board. 

The first approach is recommended, since it exhibits more flexibility and the program is more structured. For this approach, please refer to 
[Arduino program](https://github.com/teancake/Indoor-Air-Quality-Monitoring-and-Control-System/tree/master/software/sensor_unit_software/officenv_arduino_v2) and [ESP8266 program](https://github.com/teancake/Indoor-Air-Quality-Monitoring-and-Control-System/tree/master/software/sensor_unit_software/officenv_esp12ef_v1) in the [Indoor-Air-Quality-Monitoring-and-Control-System](https://github.com/teancake/Indoor-Air-Quality-Monitoring-and-Control-System) repository, respectively. 
If you insist to use the second approach, please leave the original firmware in the ESP8266 chip as it is and use [Arduino program](https://github.com/teancake/Indoor-Air-Quality-Monitoring-and-Control-System/tree/master/software/sensor_unit_software/officenv_arduino_v1) for the Arduino board. In this way, you may also need a TCP server to receive the data from the sensor, an example of the server program is [here, publish_office_air_quality.py](https://github.com/teancake/Indoor-Air-Quality-Monitoring-and-Control-System/tree/master/software/server_software) in the [Indoor-Air-Quality-Monitoring-and-Control-System](https://github.com/teancake/Indoor-Air-Quality-Monitoring-and-Control-System) repository.

### The Finished Board ###
<img src="https://github.com/teancake/Air-Quality-Monitor/blob/master/hardware_finished_top.jpg" alt="top" width="200px"> 
<img src="https://github.com/teancake/Air-Quality-Monitor/blob/master/hardware_finished_bottom.jpg" alt="top" width="200px">

