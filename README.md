# toshiba-seiya-mqtt
toshiba seiya wifi gateway to mqtt

Arduino c++ version of https://github.com/toremick/shorai-esp32 toshiba wifi gateway using ESP32
Addition of ability to telnet to esp32 and see data sent to/from toshiba a/c unit
Supports OTA updates from Arduino IDE

This works great for me, but is at your own risk!

*********Added revised version for esp8266, untested on ac unit but connects ok and sends and receives data on serail port ok

Revised version of ESP32 to improve mqtt stability issues and fix bug with seiya initial handshake timing
