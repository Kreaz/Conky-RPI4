# Conky-RPI4
Disclaimer!! This is not my work. The guide I followed was Don from Novaspirit Tech. I only tweaked the script so it will run on my RPI4B 4g. I am doing this for my own convenience.

- Install Conky
```
sudo apt-get install conky-all
```
- Download config file
```
wget -O /home/pi/.conkyrc https://raw.githubusercontent.com/Kreaz/Conky-RPI4/main/.conkyrc
```
- Creating a shell script to start conky
```
wget -O /usr/bin/conky.sh https://github.com/Kreaz/Conky-RPI4/blob/23487170c5347fe1153ae0fae792a0da378329a6/conky
```
- Create a desktop entry to autostart the script
```
wget -O /etc/xdg/autostart/conky.desktop https://raw.githubusercontent.com/Kreaz/Conky-RPI4/main/conky.desktop
```


