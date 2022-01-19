I intended to use headless setup using Ubuntu 20.3. There are some experient which I hope could save time for who need it. Actually, headless installing is quite headdache so I recommend using monitor instead. 
I didn't have keyboard and mouse (actually I had but they are wireless which are not suitable for Raspberry Pi)

Some notes:
+ Ubuntu desktop version does not init SSH in setting up so we can't remote access for headless setup.
+ With Raspberry Pi OS, it is quite easier we can add file named ssh (without extension) to enable SSH service to install headless
https://www.raspberrypi.com/documentation/computers/remote-access.html
+ I installed Ubuntu server version:
- install Raspberry Pi Imager tool --> which provides Advanced Options via hot key
- Download Ubuntu server image
- Flash to SD card
- Access flashed SD card to setup wifi network via "network-config" file. Be carefull with tab space (2 spaces) which can cause error when setting up.
- Start Raspberry Pi and access via SSH with default username/password: "ubuntu"

Notes: first installing time, it's quite long so you need wait 15m and restart again to enable wireless connection and ssh 