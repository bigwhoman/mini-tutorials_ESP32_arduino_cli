# mini-tutorials_Web_Server_ESP32
Today we are going to run a webserver on ESP32 module. <br>
The setup is on Ubuntu 22.04.
### Installing requirements 
First, we need to install arduino IDE 
```shell
   curl -fsSL https://raw.githubusercontent.com/arduino/arduino-cli/master/install.sh | sh
```
Now launch vscode and install the vscode-arduino extension.<br>
Change the setting to use the arduino-cli.
```shell
   arduino-cli config init
   sudo vim .arduino15/arduino-cli.yaml
```
Now add the library to board manager :
```shell
   board_manager:
     additional_urls:
       - https://dl.espressif.com/dl/package_esp32_index.json
```
after that update the arduino core and install esp32 package
```shell
    arduino-cli core update-index
    arduino-cli core install esp32:esp32
```
