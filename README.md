# Web page converts speech into text:
https://nadaalmehdar1999.github.io/speech-task-ESP32-module-operation-algorithm/

1-	Convert audio to Arabic text:
The task of designing and building a web page has been accomplished to test the conversion of text-to-speech for the robotic communication system and to test the recognition of the Arabic language of the Lysian communication system using notebook and programming languages HTML , CSS  and JS.

2-	ESP32 module operation algorithm:

-	the required materials:
 1-ESP32 . module
 2-USB cable
 3-Arduino IDE

Step 1: Download and install the Arduino IDE.
Step 2: After installation, open the IDE and go to Files -> Preferences and open the Preferences window and see “Additional Panel Manager URL”.
Step 3: You just have to paste the URL below into this box
https://dl.espressif.com/dl/package_esp32_index.json
Step 5: Now go to Tools->Board->Board Manager and find ESP32 and press install then the installation will take place.

-	Now to program the ESP32 using the Arduino IDE:

Step 1: First of all, connect the ESP32 to your computer using a micro-USB cable.
Step 2: Now you have to select your forum; So go to Tools->Boards and select "ESP32 Dev Module".
Step 3: Now open device manager and check which ESP32 com port is connected. Here, my ESP is connected to port 6.
Step 4: Open the Arduino IDE again and paste the given LED blink program:
int LED_BUILTIN = 2;
void setup() {
pinMode (LED_BUILTIN, OUTPUT);
}
void loop() {
digitalWrite(LED_BUILTIN, HIGH);
delay(1000);
digitalWrite(LED_BUILTIN, LOW);
delay(1000);
}
In ESP32, the internal LED is connected to pin no. 2; so I define that pin of ESP as high or low. This code makes LED blink every 1 second.
Step 5: To upload the code in ESP32, click on the upload button.
After uploading the code, you will see a window like this and finds “Done uploading.”
After going through the above steps properly, you can blink LED using ESP32-
Complete code is given below:

int LED_BUILTIN = 2;
void setup() {
pinMode (LED_BUILTIN, OUTPUT);
}
void loop() {
digitalWrite(LED_BUILTIN, HIGH);
delay(1000);
digitalWrite(LED_BUILTIN, LOW);
delay(1000);
}
