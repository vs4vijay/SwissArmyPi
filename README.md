# SwissArmyPi

```
 o-o                           O                     o--o  o-O-o 
|              o              / \                    |   |   |   
 o-o  o   o   o  o-o o-o     o---oo-o o-O-o o  o     O--o    |   
    |  \ / \ / |  \   \      |   ||   | | | |  |     |       |   
o--o    o   o  | o-o o-o     o   oo   o o o o--O     o     o-O-o 
                                               |                 
                                            o--o                 
 ```

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
 

### Use-Cases & Utilities
- WiFi Cracker (Patched Firmware Required, Please see below instructions)
  - `sudo apt-get install aircrack-ng`
  - `sudo airmon-ng start wlan0`
- `reaver`
- `wifite`
- Fake AP - Wifi Phishing
  - Wifiphisher - https://github.com/wifiphisher/wifiphisher
    - **Need two wireless card**
    - `sudo apt-get install -y python-setuptools hostapd`
    - `sudo python setup.py install`
    - `sudo wifiphisher`
  - Fluxion - https://github.com/FluxionNetwork/fluxion.git
- FM Transmitter
- Metasploit - https://null-byte.wonderhowto.com/how-to/raspberry-pi-metasploit-0167798/
- Pi As Mass Storage
- Sniffing - `bettercap`
- WiFi Jammer/Deauther - `kickthemout`
- `poinsontap`
- USB Rubber Ducky
- War-driving
- Password Cracker


### Patch Broadcom Chipset Firmware
- Broadcom Chipsets(`BCM*`) 
- 


### Extra Tools
- cmatrix
- python3-gpiozero
- mosh
- nmap - `sudo apt-get install nmap`


### General Problems
- Set keyboard layout in file: `sudo nano /etc/default/keyboard`


### Other projects like this
- http://pwnpi.sourceforge.net/
- https://github.com/pwnieexpress/raspberry_pwn
- 
