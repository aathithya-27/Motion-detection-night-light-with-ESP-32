<h1 align="center">Hi 👋, I'm Aathithya P R</h1>
<h3 align="center">A passionate frontend developer and Software developer from India</h3>

- 🔭 I’m currently working on [IoT Motion Sensor Camera using ESP32-CAM & Telegram Bot](https://github.com/aathithya-27/Motion-detection-night-light-with-ESP-32)

- 🌱 I’m currently learning **Telegram Bot API, ESP-IDF, MQTT, Advanced Embedded C++**

- 👯 I’m looking to collaborate on **Smart Home & IoT Automation Projects**

- 👨‍💻 All of my projects are available at [https://aathithyapr-portfolio.netlify.app/](https://aathithyapr-portfolio.netlify.app/)

- 💬 Ask me about **ESP32, PIR Sensors, DHT11, Arduino IDE, Telegram Bot, GPIO circuits**

- 📫 How to reach me **ironaathithya@gmail.com**

- 📄 Know about my experiences [https://aathithyapr-portfolio.netlify.app/](https://aathithyapr-portfolio.netlify.app/)

- ⚡ Fun fact **I automated my room to notify me on Telegram when there's motion and to turn on/off light through telegram 😄**

<h3 align="left">Connect with me:</h3>
<p align="left">
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://www.arduino.cc/" target="_blank" rel="noreferrer"> <img src="https://cdn.worldvectorlogo.com/logos/arduino-1.svg" alt="arduino" width="40" height="40"/> </a> <a href="https://www.cprogramming.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="c" width="40" height="40"/> </a> <a href="https://www.figma.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/figma/figma-icon.svg" alt="figma" width="40" height="40"/> </a> <a href="https://firebase.google.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/firebase/firebase-icon.svg" alt="firebase" width="40" height="40"/> </a> <a href="https://www.linux.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/> </a> <a href="https://nodejs.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original-wordmark.svg" alt="nodejs" width="40" height="40"/> </a> <a href="https://opencv.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/opencv/opencv-icon.svg" alt="opencv" width="40" height="40"/> </a> <a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg" alt="pandas" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> </p>

<p><img align="center" src="https://github-readme-stats.vercel.app/api/top-langs?username=aathithya-27&show_icons=true&locale=en&layout=compact" alt="aathithya-27" /></p>


Here’s an overview of this IoT-based ESP32 CAM project:

We will create a Telegram bot for the conversation with the ESP32-CAM;
When we send the message /photo to the ESP32-CAM bot, the ESP32-CAM board receives the message, takes a new photo, and sends it to the Telegram bot;
You can send the message /photoWithFlash to turn on ESP32-CAM’s LED flash and Lamp while capturing the photo;
You can activate/deactivate the PIR sensor by sending the message /motionOn or /motionOff, if the motion sensor is active, it will keep on sending photos, whenever it senses any motion;
You can control an AC lamp by sending the message /lightOn or /lightOff;
You can monitor the LIVE room temperature on the Telegram app by sending the message /weather;
You can send the /start message to receive a welcome message with all the commands to control the ESP32CAM;
The ESP32-CAM will only respond to messages coming from your Telegram account ID.

Required Components for ESP32CAM Project

![ESP32CAM-PIR-Motion-Sensor-Telegram-P4-1024x483](https://github.com/aathithya-27/Motion-detection-night-light-with-ESP-32/assets/127311233/d6a750d8-5f73-47e3-a11d-2b6b1b58af4f)

ESP32 CAM
PIR sensor
DHT11 Sensor
220-ohm 0.25watt Resistors – 2 no
1k 0.25watt Resistors – 2 no
1N4007 Diode
BC547 NPN Transistor – 2 no
LED 5mm – 2no
5V SPDT Relay
2-pin Terminal connectors (2 no)
SPDT slide switch
AC to DC converter 5M05 5V
FTDI232 TTL converter.

Circuit of the ESP32 CAM PIR Sensor Project
![ESP32CAM-PIR-Motion-Sensor-Circuit-P7-1024x576](https://github.com/aathithya-27/Motion-detection-night-light-with-ESP-32/assets/127311233/408a9bdf-da5c-4164-afa7-12d862f85630)

In the circuit, I have used an AC to DC converter to supply 5V to the circuit.

The PIR sensor connected with the GPIO13 through a BC547 NPN transistor. And to control the relay we have used GPIO12.

The DHT11 sensor is connected with the GPIO2 of ESP32CAM.

By turning on the slider switch connected across GPIO0 and GND, we can go to program mode. Then we can program the ESP32CAM using an FTDI232 TTL converter as shown in the circuit.
![PIRSensor-pin-768x522](https://github.com/aathithya-27/Motion-detection-night-light-with-ESP-32/assets/127311233/28d07d1e-844a-4e6f-a18b-f5fab87f67a5)

You can set the delay and sensitivity of the PIR sensor as per your requirement.


PCB Layout for ESP32CAM Motion Sensor Camera
![TOP_PCB-ESP32CAM-PIR-Sensor-1024x534](https://github.com/aathithya-27/Motion-detection-night-light-with-ESP-32/assets/127311233/592844c6-9da9-4ff5-8da9-aea999731f31)
![BOTTOM_PCB-ESP32CAM-PIR-Sensor-1024x534](https://github.com/aathithya-27/Motion-detection-night-light-with-ESP-32/assets/127311233/95d2c6b3-f47c-484b-b995-ccb152e13d77)

Please download the PCB layout, then print it on the A4 page.

Please check the PCB size while printing, it should be the same as mentioned in Layout.

![ESP32CAM-PIR-Motion-Sensor-Telegram-P1-1024x733](https://github.com/aathithya-27/Motion-detection-night-light-with-ESP-32/assets/127311233/51478691-d87a-40f9-aacc-64f2734fe2f7)

IoT-based motion camera using ESP32CAM.
Explained the Circuit of the ESP32 CAM PIR motion camera.
How to make the IoT-based motion camera on Zero PCB.
Create Telegram BOT for the ESP32-CAM
Programming ESP32 CAM motion detector camera.
PIR motion sensor security camera connection


How to Create a Telegram Bot for ESP32 CAM
Steps to create Telegram Bot for the conversation with the ESP32-CAM.
![ESP32CAM-PIR-Motion-Sensor-Telegram-P3](https://github.com/aathithya-27/Motion-detection-night-light-with-ESP-32/assets/127311233/8b19ff19-e48a-4dad-bf21-66054f1c9eae)

Go to Google Play or App Store, download, and install the Telegram app.

1. Search for “botfather” and click on the BotFather (t.me/botfather) and click on START.

2. Click or type /newbot and enter a unique name for the bot.

3. Enter a unique username for the BOT. (It must end in “bot”.)

4. You will get an HTTP API BoT token. Save the bot token as you’ll need it so that the ESP32CAM can interact with the bot.

Note: The bot token is a very long string. So copy the complete token or, you can go to the Telegram Web Interface to copy the bot token from there.

Get Your Telegram User ID
![ESP32CAM-PIR-Motion-Sensor-Telegram-P2](https://github.com/aathithya-27/Motion-detection-night-light-with-ESP-32/assets/127311233/8199d601-8541-42c3-9e5e-d598b1f2cfa9)

1. Search for “myidbot” ( t.me/myidbot ) in the Telegram app.

2. Click on Start or Restart.

3. Click or Type “/getid“.

4. You will get a reply back with your user ID. Save that user ID, as you’ll have to update it in the code.

Note: Click on the correct IDBot with the blue logo (as shown in the picture).

Program ESP32 CAM with Arduino IDE
![ESP32CAM-PIR-Motion-Sensor-Telegram-P13-1024x581](https://github.com/aathithya-27/Motion-detection-night-light-with-ESP-32/assets/127311233/e9544a9f-ccc9-41f4-b674-0e4a8d2ed8c1)
To program the ESP32CAM, first, turn on the slider switch to connect GPIO0 with GND. Then connect the FTDI232 (5V) with ESP32CAM as per the circuit.

Preparing Arduino IDE
For this IoT-based project, I have used the Arduino IDE to program ESP32 CAM.

First update the Preferences –> Aditional boards Manager URLs: https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_dev_index.json, http://arduino.esp8266.com/stable/package_esp8266com_index.json

Then install the ESP32 board (2.0.5) from the Board manager or Click Here to download the ESP32 board.
Download the required libraries from the following links:
UniversalTelegramBot Library (1.3.0)
ArduinoJson Library (6.20.0)
DHT Library (1.4.4)
The source code is given above---

In the code, you have to update the following details.

![Code-ESP32CAM-PIR-Motion-Sensor-Telegram-1024x338](https://github.com/aathithya-27/Motion-detection-night-light-with-ESP-32/assets/127311233/e4cc3df8-c872-423f-a6fc-6314729fdd19)


Enter the WiFi Credentials. ( WiFi Name & WiFi Password )
// Replace with your network credentials
const char* ssid = ""; //WiFi Name
const char* password = ""; //WiFi Password
Enter the Telegram User ID and Bot token.
// Initialize Telegram BOT
String chatId = "XXXXXXXXXX";
String BOTtoken = "XXXXXXXXXX:XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX";


After doing these changes, please upload the code to ESP32CAM.
![Arduino-IDE-setting-for-ESP32CAM-P1](https://github.com/aathithya-27/Motion-detection-night-light-with-ESP-32/assets/127311233/6d5f9b42-e7c5-4534-b1b2-ec42cadb8408)

Under the Tools menu, select Board: “AI Thinker ESP32-CAM“, Partition Scheme: “Huge APP (3MB No …), and proper PORT.

Now click on the upload button.

After programming the ESP32CAM, turn off the slider switch to exit from program mode and reset the ESP32CAM.

Connecting PIR, DHT11, Lamp & AC supply with PCB
![ESP32CAM-PIR-Motion-Sensor-Telegram-P6-1024x576](https://github.com/aathithya-27/Motion-detection-night-light-with-ESP-32/assets/127311233/d2b91888-9dc0-4a30-886b-cecfe805c5cd)

Now connect the PIR sensor, DHT11, lamp, and AC supply as per the above diagram.

Please take proper safety precautions while connecting the AC voltage.

Testing the ESP32CAM Motion Sensor Camera
Now, go to your Telegram app, and open a conversation with your bot (Tap on the BOT name from the BotFather window). Send the following commands and see the bot responding:

![ESP32CAM-PIR-Motion-Sensor-Telegram-P11-1024x581](https://github.com/aathithya-27/Motion-detection-night-light-with-ESP-32/assets/127311233/71cbb1cb-3c56-476d-b80f-15af794ec70a)

/start : Shows the welcome message with the valid commands;
/photo : Capture a new photo and sends it to your Telegram account.
/photoWithFlash : Capture a new photo with Flash.
/lightOn : Turn on the AC Lamp connected with relay.
/lightOff : Turn off the AC Lamp connected with relay.
/motionOn: Activate the PIR Motion Sensor.
/motionOff : Deactivate the PIR Motion Sensor.
/weather : Sends Live Temperature & Humidity reading from the DHT11 sensor.


![ESP32CAM-PIR-Motion-Sensor-Telegram-P11-1024x581](https://github.com/aathithya-27/Motion-detection-night-light-with-ESP-32/assets/127311233/c39e2486-840e-4e13-9e03-c73286daa187)

If you try to interact with the bot from another Telegram account, you will get the “Unauthorized user” message.

I hope you like this IoT-based PIR Motion Sensor Camera using ESP32CAM and Telegram.
