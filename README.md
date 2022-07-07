![](https://img.shields.io/github/stars/pandao/editor.md.svg) ![](https://img.shields.io/github/forks/pandao/editor.md.svg) ![](https://img.shields.io/github/tag/pandao/editor.md.svg) ![](https://img.shields.io/github/release/pandao/editor.md.svg) ![](https://img.shields.io/github/issues/pandao/editor.md.svg) ![](https://img.shields.io/bower/v/editor.md.svg)

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

```
this is test code 

```

Overview of our Project <br>

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



