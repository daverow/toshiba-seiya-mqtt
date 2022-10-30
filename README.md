# toshiba-seiya-mqtt
toshiba seiya wifi gateway to mqtt

Arduino c++ version of https://github.com/toremick/shorai-esp32 toshiba wifi gateway using ESP32
Addition of ability to telnet to esp32 and see data sent to/from toshiba a/c unit
Supports OTA updates from Arduino IDE

This works great for me, but is at your own risk!

*********Added revised version for esp8266, untested on ac unit but connects ok and sends and receives data on serail port ok

Revised version of ESP32 to improve mqtt stability issues and fix bug with seiya initial handshake timing

For ESP8266 Wemos type devices that have integral usb to serial on board there are issues with the serial port usage.
Use the esp8266 wemos version
Serial.swap(); //remap tp pins 15(tx) and 13(rx) for connection to ac unit,but use rx only from air con unit
  // but cannot use tx pin 15 for tx as level converter holds pin high and stops esp8266 boot
  //so use serial1 to tx to air con unit (gpio2)
  //no debug serial port available
  //so use gpio2 (wemos D4) tx  to air con and pin 13 (wemos D7) rx from aircon unit

