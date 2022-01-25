# Conky-RPI4
Disclaimer!! This is not my work. The guide I followed was Don from Novaspirit Tech. I only tweaked the script so it will run on my RPI4B 4g. I am doing this for my own convenience.

- Install Conky
```
$ sudo apt-get install conky-all
```
- Download config file
```
$ wget -O /home/pi/.conkyrc https://github.com/Kreaz/Conky-RPI4/blob/main/.conkyrc
```
- Creating a shell script to start conky
```
$ sudo nano /usr/bin/conky.sh
```
- Then paste this script:
```
#!/bin/sh
(sleep 4s && conky) &
exit 0
```
- Save and exit.

- Create a desktop entry to autostart the script
```
$ sudo nano /etc/xdg/autostart/conky.desktop
```
- Then paste this into the file:
```
[Desktop Entry]
Name=conky
Type=Application
Exec=sh /usr/bin/conky.sh
Terminal=false
Comment=system monitoring tool.
Categories=Utility;
```
- Save and exit.


