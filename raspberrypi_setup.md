# Configuring the Raspberry pi
Get the OS (Operating System) image you want to install from the official website: [Raspberry Pi OS](https://www.raspberrypi.org/software/operating-systems/). \
Keep in mind the hardware limitations of the Pi you are using when choosing the system. Being too greedy will only lead to a frustrating experience. Also the SD card should be a verified one as some instances of the pi not booting are due to incompatible SD cards.\
To write the chosen OS to the SD card use the [Raspberry Pi Imager](https://www.raspberrypi.org/software/). You could skip the first step as the Pi Imager allows you to download the OS directly during the installation, but that makes the process **MUCH** longer.\
As a personal preference I usually format the SD cards to EXFAT not FAT32.

***Pi Imager default screen*** 
![default_screen](img/Screenshot%202021-03-21%20090302.png)

Select "CHOOSE OS" option first to add the OS to install.

***Operating System selection pop out window***
![install_OS](img/Screenshot%202021-03-21%20100713.png)

To install the downloaded image scroll to the very bottom and select "Use custom".

---
## If you installed a version of Raspberry Pi OS (previously Raspbian)

### At first boot

The initial login credentials are

````sh
user: pi
password: raspberry
````

Once logged in go straight to the configuration menu
````sh
$ sudo raspi-config
````
You get this graphical interface:
![main_menu](img/Screenshot%202021-03-14%20104132.png)

You can go ahead and press ENTER to select the first option "System Options". The newer models of pi boards have WiFi connectivity so it's a great way to start updating the system right away if ethernet isn't available.


## If you installed Ubuntu for Raspberry Pi

### At first boot