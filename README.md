<p align="center"><img alt="PICTURE logo" src="https://i.imgur.com/QVJjB9k.jpg" width="200"></p>

<p align="center">
  🐦<a href="https://twitter.com/244v234">Twitter</a>
| 📺 <a href="https://www.youtube.com/channel/UC5yaB0VU_u4sY-DiE0BGuSw/featured?view_as=subscriber">YouTube</a>
| 🌍 <a href="http://wifiphisher.tk">wifiphisher.tk</a><br>
<br></p>

## ESP8266 WifiPhisher
Wifiphisher can be further used to mount victim-customized web phishing attacks against the connected clients in order to capture credentials (e.g. from third party login pages or WPA/WPA2 Pre-Shared Keys) by using an inexpensive ESP8266 WiFi SoC (System On A Chip).

## Main feature
* The deauthentication attack, is used to disconnect devices from their WiFi network.	
* It is capable of performing a social engineering attack to get a secret WPA / WPA2 password
* The "Login" scenario provides a simple way to capture credentials from the social network Facebook.

## Video demo
[![Watch the video](https://img.youtube.com/vi/CjbRaxBsODA/0.jpg)](https://youtu.be/CjbRaxBsODA)

## Pinout
<p><img alt="PICTURE logo" src="https://hackster.imgix.net/uploads/attachments/1212694/244v234_pe3ov4zwv9_xBZN30K1NU.jpg?auto=compress%2Cformat&w=740&h=555&fit=max" width="200"></p>

## Installation  
***YOU ONLY NEED TO DO ONE OF THE INSTALLATION METHODS!***

#### 1.Uploading the bin files  

* Download the current release from [releases](https://github.com/244v234/ESP8266-WifiPhisher/releases)  

* Upload using the ESP8266 flash tool of your choice:  
	- [nodemcu-flasher](https://github.com/nodemcu/nodemcu-flasher) [Windows only]  
	- [esptool-gui](https://github.com/Rodmg/esptool-gui) [Windows, MacOS]  
	- [esptool](https://github.com/espressif/esptool) [Windows, MacOS, Linux]  

Make sure your settings are correct for your board. Most boards come with 4mb flash and sometimes you have to hold the flash button down while plugging it in and hold it until the flashing process started.  
Also make sure you select the right com-port, the right upload size (mostly 4mb) and the correct .bin file.  
If it's not working, you can try using the Arduino as descriped below.

#### 2.Compiling the source with Arduino
First you have to install and open the Arduino IDE.
* Add the required [libraries](https://drive.google.com/drive/folders/1QKlt-UVW6BszD1YrvQ47xcYCMHJUfeuS?usp=sharing)
* In Arduino go to File -> Preferences add both URLs in Additional Boards Manager URLs https://raw.githubusercontent.com/SpacehuhnTech/arduino/main/package_spacehuhn_index.json
* Go to Tools -> Board -> Boards Manager, search "deauther" and install Deauther ESP8266 Boards
* Select your board at Tools -> Board and be sure it is at Deauther ESP8266 Boards (and not at ESP8266 Modules)!
* Download the source code for this project from the releases page. You can also clone the project to get the latest changes, but you will also get the latest bugs ;)
* Extract the whole .zip file, and open ESP8266-WifiPhisher.ino with Arduino.
* Check your upload settings and press upload!

## :octocat: Contribute
All contributions are welcome! Code, documentation, graphics, or even design suggestions are welcome; use GitHub to its fullest. Submit pull requests, contribute tutorials -- whatever you have to offer, it'll be appreciated

## Under Development
Currently, the ESP8266 WifiPhisher has limited software capabilities. New firmware features will be added over time and will eventually reach the point where this project becomes the smallest hacking machine.

## Disclaimer
Usage of ESp8266 Wifiphisher for attacking infrastructures without prior mutual consistency can be considered as an illegal activity. It is the final user's responsibility to obey all applicable local, state and federal laws. Authors assume no liability and are not responsible for any misuse or damage caused by this program.

## Note
* Beware of websites pretending to be related to the ESP8266 WifiPhisher Project. They may be distributing malware.
* WifiPhisher does not work on esp32. There is no way to inject packets on the ESP32

##### This source code is built on [Deauther](https://github.com/SpacehuhnTech/esp8266_deauther)
