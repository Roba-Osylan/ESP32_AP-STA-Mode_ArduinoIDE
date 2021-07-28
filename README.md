# ESP32_AP-STA-Mode_ArduinoIDE

Through this project, the ESP32 will be programmed in order to connect the robot's tablet with the ESP32 and connect the ESP32 with an existing network. The Figure below illustrates the project diagram, which shows that in order for the client (the robot) to connect to the ESP32, an SSID should be defined for the ESP32 (WiFiAccessPoint ArduinoIDE Example). Then, in order for the ESP32 to be connected to a WiFi network, an Http request must be generated (BasicHttpsClient Arduino IDE Example). 

![project diagram](https://user-images.githubusercontent.com/85955049/127399738-8e9c4418-3108-4fdb-9ef8-c09ae87f54ca.png)

**ESP32: Programming and Operating Modes**

The ESP32 can be programmed in different languages such as Arduino IDE, MicroPython and JavaScript. However, through this project the ESP32 is programmed using Arduino IDE as it is illustrated in the following section.

There are three operating modes for the ESP32, the Access Point Mode (AP), the Station Mode (STA) and the AP-STA Mode which involves both Modes together. The ESP32 in AP mode has a Wi-Fi network, SSID and IP address and hence it acts as a router for up to five stations (devices) which can receive web pages as long as they are connected to this network. In the STA mode, the ESP32 is connected to Wi-Fi router and hence it is considered as a station that acts as a web server which can deliver web pages to all other stations that are connected to the same Wi-Fi router. (Last Minute Engineers).

# Installing Board 

The process of implementing the task begins with installing the board module in Arduino IDE. First, the URL shown in the Figure below is pasted in the “Additional Boards Manager URLs” in the “Preferences” window. 
![preferences](https://user-images.githubusercontent.com/85955049/127400236-05eb975d-0b06-4064-85dc-10594e68f6cc.png)

Then from the “Boards Manager” the package “esp32” is installed as it is illustrated in the Figure below. 

![board installation](https://user-images.githubusercontent.com/85955049/127400336-ea1c9101-e10f-4794-a8d8-241d3175aabf.jpg)

After installing the esp32 package, the examples for WEMOS D1 MINI ESP32 are included. However, through this project we will use the “WiFiAccessPoint” example from “WiFi” list and the “BasicHttpsClient” from the “HTTPClient” list.

# Setting the ESP32 in AP-STA Mode

The program is uploaded under the name "ESP32-Test1" to be tested during the SYNC mission. 

