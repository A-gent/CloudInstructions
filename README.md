# CloudInstructions
AHK-based uploader system to allow my bots on the server to be remote controlled by number-based variables (utilizing a periodic timer-based scanning system that will auto-download the instructions.txt file every so often and check its value to see if we should perform any logical steps).

This repo is just to house the instructions file for my parse / updater (that changes the instructions.txt as per desired from the manifest file and then uses Portable Git for Windows to push the update to the instruction.txt housed in the Git-side repo; this repo here).

The parse / reader system will do as mentioned prior: use a timer-based system to download the instructions file every so often and then read / perform actions based upon current instruction var value.


The main pilot for this project (and where I will derive most of its usefulness) will be with my Diablo 2 Stealthbot.  Using this system, I don't have to remote in to turn the Stealthbot on or off, I can just create a separate system that will push changes to the manifest file (example: 1 for on, 0 for off) and then run the Parse / Updater to push the change to Git.  Then the timer-based parse / read system running on the server PC will eventually end up downloading the newly changed file and performing routine changes based upon the instructions value it reads. (example: turn the bot off, or turn it back on).
