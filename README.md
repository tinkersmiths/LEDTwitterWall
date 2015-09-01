# LEDTwitterWall
Software for 10 ft LED matrix sign that runs Arduino Yun pulling from twitter mentions


The board on the wall now is an Arduino Yun.

 * Twitter Integration uses: https://temboo.com/library/Library/Twitter/Timelines/LatestMention/
 * LED board is based on: https://learn.adafruit.com/guggenhat-bluetooth-le-wearable-neopixel-marquee-scrolling-led-hat-display/code

250 API calls allowed per month for free. 730 hours in a month >> 1 call every 3 hours (10800000 ms)

## Clone instructions
 * git clone 
 * create LEDTwitterWall/TwitterMentionsWall/TembooAccount.h with your creds
 * open LEDTwitterWall/TwitterMentionsWall/TwitterMentionsWall.ino sketch in Arduino IDE
 * select Tools->Board-> Arduino Yun
 * select Tools->Port->Arduino Yun WiFi (the-yun-ip)
 * Compile and upload
 * You should be good to go!

## The sketches here...
 * TwitterMentionsWall - The main project, bringing it all together
 * Console_Test	- The YUN DOES NOT SUPPORT SERIAL OVER WiFi, so you have to use the Bridge with Console.println instead to get output. This is an example to do just that.
 * TwitterTest - USB only test of the Twitter/Temboo pulling code
 * TwitterTestConsole - WiFi varient of the above, switching out Serial debug messages for Console


## Depend Libraries
 * Adafruit-GFX-Library-master.zip
 * Adafruit_NeoMatrix-master.zip
 * Adafruit_NeoPixel-master.zip
 
 
## Some useful references:
 * http://kiwitobes.com/2013/09/26/twitter-lights-and-memory-limits-with-arduino-yun/
 * https://temboo.com/library/Library/Twitter/Timelines/LatestMention/
 * https://www.arduino.cc/en/Tutorial/ConsoleRead
 * https://www.arduino.cc/en/Guide/ArduinoYun
 * http://stackoverflow.com/questions/20681318/arduino-yun-serial-communication-not-working
 * 
