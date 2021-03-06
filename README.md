# Робот Миньон - напомнит Вам о поливе растений
Arduino based Robot for plant moisture sensing.


Видео рабочего робота [youtube](https://www.youtube.com/watch?v=4_Oq1PAKOGk). 
Другие проекты от автора [yellowrobot.xyz](http://www.yellowrobot.xyz).
Оригинал [GitHub](https://github.com/evaldsurtans/robot_minion).

Robot components:

* WTV020-SD
	* 4 (+), 5 (-) -> Speaker
	* 16 -> VCC
	* 8 -> GND
	* 10 -> A2 Ardunio (digital com cable)
	* 1 -> A0 Ardunio (reset)
	* 7 -> A1 Arduion (clk)
* PIR - HC-SR501
	* D Output -> D10 Arduino
* YL-38 moisture sensor
	* A0 -> A3 Ardunio
	* Desolder power LED
* LIPO charger MCP73831T
	* Desolder Charging LED
	* Custom soldering point at charging LED (as shown in photo) -> A6 Arduino
* Arduino
	* Desolder power LED
	* Just to remember D13 is a onboard LED - very useful for debugging
	* Add header pins in order to connect FTDI programmer to USB