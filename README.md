### demo program capable of inspiring coding agents whsn using this board

## How to use it
### make sure this works
- clone this project (see instructions below)
- test your board
- if it works, this repo can be used by you AI agent to develop your app using the below prompt

### Prompt for any subsequent projects

Note: tested with claude code in vscode on Windows/git-bash with arduino-cli 1.4.1 and arduino-esp32 3.3.6

Use this context prompt
```
In this repository, a application for ESP32 with the same name as the repository 
and using the arduino-cli compilation system must be created.

arduino-cli is made available by sourcing the file /c/Users/<userpath>/arduino-cli-setup.sh.

The board uses the GT911 IC as the interface with the capacitive sensor; 
the TAMC_GT911 library must be used for this circuit.

The program to create consists of displaying a simple button on the screen 
of a reference CYD esp32-2432S032C.

The code to use as a model for initializations and library usage is here:
https://github.com/joseluu/Demo-CYD-3.2inch-ESP32-2432S032

Other ways of developing for this specific hardware combination do not work. 
Do not modify the files touch.cpp nor touch.h.

Create the file docs/done_changes.md and write in it a report/summary of all actions performed.

Compile the program using arduino-cli. 
The hardware configuration to set for compilation is: "ESP32 Dev Module"

The Arduino_GFX library must be updated directly from the GitHub repository.
The lvgl library has to be in version 8.3.11
```






## Installing this project
target board: ESP32-2432S032C

was https://fr.aliexpress.com/item/1005005138982767.html

now possibly https://fr.aliexpress.com/item/1005008599170226.html

Must install lvgl by kesvegabor version 8.3.11
After installing this library, the file ./LVGL configuration replacement file/lv_conf.h
has to be copied along the lvgl library, usually in C:\Users\<username>\Documents\Arduino\libraries
As of 2026-01024, use ESP32 3.3.6, see code about the Arduino_GFX_Library

