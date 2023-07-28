# Template WiFiManager | OTA | ESP CHIPS
![mecabotic.com](https://mecabotic.com/wp-content/uploads/2018/02/logotipo-claro.png)
[![mecabotic - ESP32_OTA_WifiManager](https://img.shields.io/static/v1?label=mecabotic&message=ESP32_OTA_WifiManager&color=blue&logo=github)](https://github.com/mecabotic/ESP32_OTA_WifiManager "Go to GitHub repo") [![stars - ESP32_OTA_WifiManager](https://img.shields.io/github/stars/mecabotic/ESP32_OTA_WifiManager?style=social)](https://github.com/mecabotic/ESP32_OTA_WifiManager) [![forks - ESP32_OTA_WifiManager](https://img.shields.io/github/forks/mecabotic/ESP32_OTA_WifiManager?style=social)](https://github.com/mecabotic/ESP32_OTA_WifiManager)  [![GitHub release](https://img.shields.io/github/release/mecabotic/ESP32_OTA_WifiManager?include_prereleases=&sort=semver&color=blue)](https://github.com/mecabotic/ESP32_OTA_WifiManager/releases/) [![License](https://img.shields.io/badge/License-GPL-blue)](#license) [![issues - ESP32_OTA_WifiManager](https://img.shields.io/github/issues/mecabotic/ESP32_OTA_WifiManager)](https://github.com/mecabotic/ESP32_OTA_WifiManager/issues)

## *Plantilla para ESP32 con WifiManager y OTA*

Portal cautivo de wifimanager (2 campos)

 - Cuadro de texto (String)

 - Cuadro de texto (número)

**Entrará en modo de configuración si:**
 - No puede conectarse al WiFi
 - No existe una configuración en el sistema de archivos (FS)
 - El usuario ha hecho "doble reset"
   
   (presionó el botón de reinicio dos veces)
   
**ESP32**\
[![view - Documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](https://github.com/espressif/arduino-esp32/tree/master "https://github.com/espressif/arduino-esp32/tree/master")
## Definiciones de Bibliotecas
**#include  <WiFi.h>**

*Biblioteca Wifi*

http://www.arduino.cc/en/Reference/WiFi

https://github.com/arduino-libraries/WiFi

**#include  <FS.h>**

*Biblioteca File System | Acceso al sistema de archivos*\
[![view - Documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](https://github.com/espressif/arduino-esp32/tree/master/libraries/FS "https://github.com/espressif/arduino-esp32/tree/master/libraries/FS")


**#include  <SPIFFS.h>**

*SPIFFS es un sistema de archivos para las memorias SPI Flash NOR que utiliza el ESP3*2\
[![view - Documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](https://github.com/espressif/arduino-esp32/tree/master/libraries/SPIFFS "https://github.com/espressif/arduino-esp32/tree/master/libraries/SPIFFS")


**#include  <HTTPClient.h>**

*Biblioteca para realizar fácilmente solicitudes HTTP GET, POST y PUT a un servidor web.*

Funciona con cualquier clase derivada de Client, por lo que cambiar entre Ethernet, WiFi y GSMClient requiere cambios de código mínimos.\
[![view - Documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](https://github.com/espressif/arduino-esp32/tree/master/libraries/HTTPClient "https://github.com/espressif/arduino-esp32/tree/master/libraries/HTTPClient")

**#include  <HTTPUpdate.h>**

*Permite usa con y sin https*\
[![view - Documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](https://github.com/espressif/arduino-esp32/tree/master/libraries/HTTPUpdate "https://github.com/espressif/arduino-esp32/tree/master/libraries/HTTPUpdate")


**#include  <WiFiClientSecure.h>**\
[![view - Documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](https://github.com/espressif/arduino-esp32/tree/master/libraries/WiFiClientSecure "https://github.com/espressif/arduino-esp32/tree/master/libraries/WiFiClientSecure")



**#include  "cert.h"**

*Biblioteca local, certificados TLS - SSL*

**#include  <WiFiManager.h>**

*Portal cautivo para configurar el WiFi*

Puede instalarse desde el administrador de bibliotecas (Busca "WifiManager", instala la versión Alpha)\
[![view - Documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](https://github.com/tzapu/WiFiManager "https://github.com/tzapu/WiFiManager")



**#include  <ESP_DoubleResetDetector.h>**

*Una biblioteca para verificar si el botón de reinicio se ha presionado dos veces*

Puede utilizarse para habilitar el modo de configuración

Puede instalarse desde el administrador de bibliotecas (Busca "ESP_DoubleResetDetector")\
[![view - Documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](https://github.com/khoih-prog/ESP_DoubleResetDetector)



**#include  <ArduinoJson.h>**

*ArduinoJson se utiliza para analizar y crear el archivo de configuración.*

Busca "ArduinoJson" en el administrador de bibliotecas de Arduino\
[![view - Documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](https://github.com/bblanchon/ArduinoJson)




## Constantes:

**#define  URL_fw_Version**  "https://url-aqui/archivo-bin-version.txt"

**#define  URL_fw_Bin**  "https://url-aqui/archivo-firmware.bin"

**#define  JSON_CONFIG_FILE  "/tu_config.json"**

 - ***Configuracion wifi por Defecto Mecabotic Hardware***

!wm.autoConnect("**MecaboticAP**", "**Soymecaboter.777**")


## Contacto:
[![Ask Me Anything !](https://img.shields.io/badge/Ask%20me-anything-1abc9c.svg)](https://github.com/orgs/mecabotic/discussions)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
[![GPLv3 license](https://img.shields.io/badge/License-GPLv3-blue.svg)](http://perso.crans.org/besson/LICENSE.html)
