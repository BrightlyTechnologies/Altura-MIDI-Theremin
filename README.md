# Altura-MIDI-Theremin
Source code and binaries for the clever controller that emulates a theremin

To get the latest release onto your altura
0. Obtain and setup avrdude
1. Download Altura_2.1.1.ino.hex
2. Connect your altura to your computer through a usbtiny programmer.
3. Open up a command prompt and navigate to the folder where you have the hex file.
4. use the command avrdude -c usbtiny -p m328p -B 1 -V -U flash:w:Altura_2.1.1.ino.hex

To make custom edits to the source code.
-1. Obtain and setup the latest version of the Arduino IDE.
0. Obtain the arduino MIDI library from forty-seven effects.
1. Download Altura_2.1.1.ino and open it with Arduino (Arduino should create a folder for it and move it inside)
2. Make your edits.
3. When you're done click verify and wait for it to finish.
4. Altura_2.1.1.ino.hex should be created somewhere in your appdata folder(if you're having trouble finding it make sure you are showing hidden folders in folder options)
5. Follow the instructions for how to get the latest release from step 2.