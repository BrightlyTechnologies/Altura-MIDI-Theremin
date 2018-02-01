# Altura-MIDI-Theremin
Source code and binaries for the clever controller that emulates a theremin

To get the latest release onto your altura
1. Obtain and setup avrdude
2. Download Altura_[version number].ino.hex. Always use the latest release!
3. Move Altura_[version number].ino.hex into the same folder as avrdude.exe
4. Connect your Altura to your computer through a usbtiny programmer.
5. Open up a command prompt and navigate to the folder where you have avrdude.exe.
6. Enter this command: "avrdude -c usbtiny -p m328p -B 1 -V -U flash:w:Altura_[version number].ino.hex" If you copy-and-paste this line, be careful to edit the file name to exactly match the name of your hex file!

To make custom edits to the source code.
1. Obtain and setup the latest version of the Arduino IDE.
2. Obtain the arduino MIDI library from https://github.com/FortySevenEffects.
3. Download Altura_[version number].ino and open it with Arduino (Arduino should create a folder for it and move it inside)
4. Make your edits.
5. When you're done click verify and wait for it to finish.
6. Altura_[version number].ino.hex should be created somewhere in your appdata folder. (If you're having trouble finding it make sure you are showing hidden folders in folder options.)
7. Follow the instructions for "how to get the latest release", above, from step 3.
