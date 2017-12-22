# Tensorflow Environment on Raspberry Pi 2 & 3

Install a fresh copy of [Raspbian OS](https://www.raspberrypi.org/downloads/raspbian/) on an SD card, and power on your Pi. Crosscompiling takes a long time, and requires you to use a swap file which is time consuming when you want to get Tensorflow up and running on you Pi.

```
sudo apt-get update
```

```
sudo apt-get install python-pip python-dev
```

Download the tensorflow wheel

```
wget https://github.com/samjabrahams/tensorflow-on-raspberry-pi/releases/download/v1.1.0/tensorflow-1.1.0-cp27-none-linux_armv7l.whl
```
I want to use Python 2, so I'm using the python2.7 wheel provided by [samjabrahams.](https://github.com/samjabrahams/tensorflow-on-raspberry-pi#installing-from-pip) He has provided wheel for Python 3 as well, head there if you want to you Python 3.
```
sudo pip install tensorflow-1.1.0-cp27-none-linux_armv7l.whl
```

```
sudo pip uninstall mock
```

```
sudo pip install mock
```


Reference:

https://github.com/samjabrahams/tensorflow-on-raspberry-pi#installing-from-pip

https://petewarden.com/2017/08/20/cross-compiling-tensorflow-for-the-raspberry-pi/
