# SwissArmyPi

### Hardware Required
- Raspberry Pi (I am using Raspberry Pi Zero W)
- SD Card (I am using 16 GB)
- MicroUSB Cable
- WiFi Card (The inbuilt Wireless card doesn't support monitor mode, We need external wifi card. e.g. TP-LINK WN722N)

```
.-------------------------.
| oooooooooooooooooooo J8 |
| 1ooooooooooooooooooo   |c
---+       +---+ PiZero W|s
 sd|       |SoC|   V1.1  |i
---+|hdmi| +---+  usb pwr |
`---|    |--------| |-| |-'
```

### Basic Installation
- Download Linux Image, Options are:
  - Raspbian
  - RetroPie
- Flash Image to SD Card using Etcher(https://etcher.io/)
- Configure SSH and Ethernet Gadget mode so that we can SSH into Pi using microusb cable
- Connect Pi with USB Cable via usb port(Pi Zero W has two microusb port: one for power, second for usb)
- Once Pi boots up, Run following commands to Configure & Update the system and depedencies:
  - `sudo apt-get update`
 


### Utilities
- WiFi Cracker (Patched Firmware Required, Please see below instructions)
  - `sudo apt-get install aircrack-ng`
  - `sudo airmon-ng start wlan0`

- FM Transmitter
- Metasploit


### Patch Broadcom Chipset Firmware
Broadcom Chipsets(`BCM*`) 
- 


### General Problems
- Set keyboard layout in file: `sudo nano /etc/default/keyboard`

