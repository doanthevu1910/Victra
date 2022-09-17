# Hardware

```
CPU:                 Intel® Core™ i5-10400F
GPU:                 SAPPHIRE NITRO+ RX 580 8G G5 SE
RAM:                 Kingston FURY™ Beast 16GB (2x8GB) DDR4 2666MHz
SSD:                 XPG SX8200 Pro 512GB
Motherboard:         ASRock B460M Pro4
Audio codec:         Realtek ALC1200
Ethernet card:       Intel® Gigabit LAN
Wifi/Bluetooth card: None
```

# macOS Monterey 12.4 & OpenCore 0.8.0

https://dortania.github.io/OpenCore-Desktop-Guide

# Works
- Sleep
- Wake
- Audio
- Ethernet
- All USB ports (2.0, 3.0 & Type-C)

# Doesn't work
- AirDrop, Handoff, Continuity (native Wifi/Bluetooth card needed)

# Result
![Info](https://github.com/doanthevu1910/Victra/blob/455ae18fdad9d4f60b1b3ebc322ded52d4a9bfec/images/Screen%20Shot%202022-09-17%20at%2013.12.09.png)

# Note

Please change MLB, SystemSerialNumber, and SystemUUID using [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS).

```
<dict>
    <key>AdviseWindows</key>
    <false/>
    <key>MLB</key>
    <string>xxxxxxxxxxxxxxx</string>
    <key>ROM</key>
    <data>xxxxxxxx</data>
    <key>SpoofVendor</key>
    <true/>
    <key>SystemProductName</key>
    <string>iMac20,1</string>
    <key>SystemSerialNumber</key>
    <string>xxxxxxxxxxx</string>
    <key>SystemUUID</key>
    <string>xxxxxxxx-xxxxx-xxxxx-xxxx-xxxxxxxx</string>
</dict>
```
