### A2VGA

This project is a new hardware implementation of the work done by Mark Aikens and David Kuder on the VGA analog card for Apple2.

The card is based on RPI Pico, 74LVC245 chips and a PLD. It is all through-hole. An improvement is that an ATF22V10 is used, which has sufficient I/O lines to allow that all necessaty bits of the address bus (A0-A10) are decoded for correct switching off of the ExtROM, in case the RPI firmware is using this memory. Additionally, the nLRESET signal can be fed to pin 30 of the Pico via a jumper, in case it is needed by future firmwares.

In this v1.2 the PCB design is optimized and +5V power is added to pin 9 of the VGA connector for use by moded VGA-to-HDMI adapters. The power is fed via a resettable fuse Fu1. A standard VGA-to-HDMI can also be used by attaching a micro-USB power cable to the output of the fuse and ground.

### Acknowledgements
This is a fork of David Kuder [V2RetroComputing](https://github.com/V2RetroComputing/analog/) and [∀2 Retro Computing](https://www.v2retrocomputing.com/) project with a new board design intended to fully support his software.
The original design was posted by Mark Aikens [Apple II VGA](https://github.com/markadev/AppleII-VGA/).


