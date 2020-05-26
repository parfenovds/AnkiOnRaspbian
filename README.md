# AnkiOnRaspbian

An easy way to install Anki on your Raspberry pi

## Problem description

There are a lot of missing dependencies when you're trying to install anki on your Raspberry pi (python3-pyqt5.qtwebengine, for example). In accordance to http://archive.raspbian.org/raspbian/pool/main/p/pyqt5webengine/ there is no pyqt5-qtwebengine in the relevant directory. So, we have to put it in our system.

### How to solve it

1. Firstly, after clone this repository to your raspberry pi, you've got to cd to appropriate directory:

```
cd AnkiOnRaspbian
```
2. Then, use this command to install all missing packages (make sure you have successfully copied entire command, it's long enough!):
```
sudo dpkg -i libqt5designer5_5.11.3-4_armhf.deb libqt5help5_5.11.3-4_armhf.deb libqt5test5_5.11.3+dfsg1-1+deb10u3_armhf.deb python3-sip_4.19.14+dfsg-2_armhf.deb python3-pyqt5_5.11.3+dfsg-1+b3_armhf.deb libqt5qml5_5.11.3-4_armhf.deb libqt5webchannel5_5.11.3-2_armhf.deb python3-pyqt5.qtwebchannel_5.11.3+dfsg-1+b3_armhf.deb libqt5webengine-data_5.11.3+dfsg-2+deb10u1_all.deb libqt5quick5_5.11.3-4_armhf.deb libminizip1_1.1-8+b1_armhf.deb libqt5positioning5_5.11.3+dfsg-2_armhf.deb libre2-5_20190101+dfsg-2_armhf.deb libqt5webenginecore5_5.11.3+dfsg-2+deb10u1_armhf.deb libqt5webengine5_5.11.3+dfsg-2+deb10u1_armhf.deb libqt5quickwidgets5_5.11.3-4_armhf.deb libqt5webenginewidgets5_5.11.3+dfsg-2+deb10u1_armhf.deb python3-pyqt5.qtwebengine_5.11.3+dfsg-1+b3_armhf.deb
```
3. Install anki and use it wisely:
```
sudo apt install anki
```
