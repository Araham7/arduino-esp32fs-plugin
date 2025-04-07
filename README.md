# Arduino ESP32 filesystem uploader 

Arduino plugin which packs sketch data folder into SPIFFS filesystem image,
and uploads the image to ESP32 flash memory.

# ESP32FS Plugin Installation Guide

## Installation

### For **Windows**:

1. Make sure you're using one of the **supported versions of the Arduino IDE (Arduino 1.x.x)** and have the **ESP32 core** installed.
2. Download the tool archive from the [releases page](https://github.com/me-no-dev/arduino-esp32fs-plugin/releases/latest).
3. In your Arduino sketchbook directory, create a `tools` directory if it doesn't already exist.
4. Unpack the downloaded archive into the `tools` directory. The final path should look like:  
```
<home_dir>/Arduino/tools/ESP32FS/tool/esp32fs.jar
```
5. Restart the Arduino IDE.

> **Note for macOS (OS X):**  
> Create the `tools` directory inside `~/Documents/Arduino/` and extract the files there.

---

### For **Linux** (including Raspberry Pi):

1. Ensure you're using a **supported version of Arduino IDE (Arduino 1.x.x)** and have the **ESP32 core** installed.
2. Download the tool archive from the [releases page](https://github.com/me-no-dev/arduino-esp32fs-plugin/releases/latest).
3. Open Arduino IDE, go to `File` > `Preferences`, and **copy the Sketchbook location** (e.g., `/home/YourUsername/Arduino`).
4. Navigate to that location in your file system.
5. Create a `tools` folder (if it doesn't exist), and unzip the `ESP32FS-1.1.zip` file inside it.
6. Ensure the extracted structure looks like this:
```
/home/YourUsername/Arduino/tools/ESP32FS/tool/esp32fs.jar
```
7. Restart the Arduino IDE.

---

> **IMPORTANT NOTE:**  
> To learn how to upload SPIFFS files, you can check out the many tutorials available on YouTube.



## Usage

- Open a sketch (or create a new one and save it).
- Go to sketch directory (choose Sketch > Show Sketch Folder).
- Create a directory named `data` and any files you want in the file system there.
- Make sure you have selected a board, port, and closed Serial Monitor.
- Select *Tools > ESP32 Sketch Data Upload* menu item. This should start uploading the files into ESP32 flash file system.

  When done, IDE status bar will display SPIFFS Image Uploaded message. Might take a few minutes for large file system sizes.

## Credits and license

- Copyright (c) 2015 Hristo Gochkov (hristo at espressif dot com)
- Licensed under GPL v2 ([text](LICENSE))
- Maintained by Hristo Gochkov (hristo at espressif dot com)

## Issues and suggestions

File issues here on github, or ask your questions on the [esp32.com forum](http://esp32.com).
