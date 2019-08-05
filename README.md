# PulseSensor Visualizer Record/Playback
Version of Pulse Sensor Visualizer that will record and playback a data file.

## Recording
This sketch will work with an Arduino programmed with `PulseSensor_BPM` or `PulseSensor_BPM_Alternative` from the [PulseSensor Playground Examples](https://github.com/WorldFamousElectronics/PulseSensorPlayground/tree/master/examples)

**NOTE** Make sure that you set the `OUTPUT_TYPE` to `PROCESSING_VISUALIZER` in the Arduino sketch!

When this sketch opens, it will prompt you to select your serial port. It is the same one you used when you programmed your Arduino. When you select the port, the program will create a CSV file automatically and put it in the folder called `PulseSensor Data` inside this sketch's folder. The data is coming in from Arduino at about 50Hz.

**NOTE** The Arduino samples at 500Hz, but down-samples to the computer. The 50Hz rate is pretty accurate.

The recording will continue until the sketch is closed.

## Playback
When the sketch opens and prompts you to select a serial port, you will also have the option to select a playback file. When you select this option, a window will open to the `PulseSensor Data` folder so you can select the file you want.
The file will play until the end and then go back to the select options window.

## Keyboard commands
Press `s` or `S` to take a screenshot of the program window. The file will be saved inside this sketch folder.

