

![](https://github.com/DebankanSarkar12/Metro-Hazard-Detection-/blob/main/Img/ThinkSpeak.png)
![](https://github.com/DebankanSarkar12/Metro-Hazard-Detection-/blob/main/Img/Firebase.png)
![](https://github.com/DebankanSarkar12/Metro-Hazard-Detection-/blob/main/Img/Telegrambot.PNG)

## Project Description

Implemented a Iot project on 'Metro Safety System'.
<br> In this project,  abnormal discrepancies like fire, gas leakage, sparks, high temperature, and humidity are being checked and alerted.
<br>Developed an Android application which fetches data from Firebase Realtime database and an alert notification system that sends alert texts from Nodemcu to Telegram.


## Implementation

The NodeMcu listens on the Serial ports for commands. The commands are interpreted and used to control the sensors . 
The data collected from the sensor is sent to the ThinkSpeak and Firebase Realtime Database . On reaching a particular threshold value the sensor sends a bot message from nodemcu to tthe telegram bot created through BotFather . The data is fetched from Firebase Realtime Database to the android app . 

## Hardware Connection

| Sensor  | Port |
| ------ | ------ |
| MQ2 | A0 |
| DHT22 | D4|
| Flame|D2|
| LDR| D1 |
|Buzzer| D3 |

## Code 

```
this is test code 

```






### Overview of our Project <br>

### HARDWARE REQUIREMENTS<br>

•	Nodemcu esp8266 <br>
•	DHT22 Sensor  ( measuring temperature and humidity abnormalities)<br>
•	MQ2 Sensor  ( measuring smoke abnormalities)<br>
•	Flame Sensor <br>
•	LDR Sensor  ( measuring high light abnormalities )<br>
•	Buzzer<br>
•	Jumper Wires <br>
•	Breadboard <br>

### SOFTWARE REQUIREMENTS<br>

| Software  | Links |
| ------ | ------ |
| Arduino | https://www.arduino.cc/en/software |
| Firebase | https://firebase.google.com/ |
| ThinkSpeak | https://thingspeak.com/ |
| Telegram | https://web.telegram.org/k/ |

### Block Diagram

```seq
DHT22 Sensor->NodeMcu(Esp8266) : Sends Temperature and Humidity Reading
Flame Sensor->NodeMcu(Esp8266) : Sends Fire Reading
LDR Sensor->NodeMcu(Esp8266) : Sends Light Reading
MQ2 Sensor->NodeMcu(Esp8266) : Sends Smoke Reading
NodeMcu->Buzzer: Alert on Abnormilities
NodeMcu->Thinkspeak: Sends data to ThinkSpeak Server and displays a graph
NodeMcu-->Firebase:  Sends data to Firebase Realtime Database
NodeMcu-->Telegram Bot:  Sends Notification on Abnormilities
Firebase-->Android App: Shows Fast, Live Data on App .
```

Here is a simple flow chart:

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```


