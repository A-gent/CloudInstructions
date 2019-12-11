# CloudInstructions
AHK-based uploader system to allow my bots on the server to be remote controlled by number-based variables (utilizing a periodic timer-based scanning system that will auto-download the instructions.txt file every so often and check its value to see if we should perform any logical steps).

This repo is just to house the instructions file for my parse / updater (that changes the instructions.txt as per desired from the manifest file and then uses Portable Git for Windows to push the update to the instruction.txt housed in the Git-side repo; this repo here).

The parse / reader system will do as mentioned prior: use a timer-based system to download the instructions file every so often and then read / perform actions based upon current instruction var value.
