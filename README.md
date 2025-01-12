# ESP32-CAM

#### Arduino Example
https://github.com/espressif/arduino-esp32/blob/master/libraries/ESP32/examples/Camera/CameraWebServer/CameraWebServer.ino

### Hardware
- Board ESP32-CAM-MB adapter serial to USB
- Board ESP32-CAM contain the ESP-32S chip

#### Compatible cams

- OV2640 Cam
- OV7670 Cam
- RHYX M21-45 Support no compression (GC2145 enthält ein 1616 V x 1232 H 2MP) the trassive time is too long use only 

#### RHYX M21-45
Use the example from above and set config.pixel_format = PIXFORMAT_RGB565; // JPEG compression not supportet ignore errors in serial monitor

##### Probleme
Manchmal kommt es vor wenn man aus Asien das ESP32-CAM Board kauft das dann eine Kamera mit der Bezeichnung RHYX M21-45 dabei ist es handelt sich um eine GC2145 dies führt zu Problemen da sie keine integrierte Kompression hat und das senden in voll auflösung zu langsam ist.

###### TODO
Upgrade core for GC2145