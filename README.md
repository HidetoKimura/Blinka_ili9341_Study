# Blinka_ili9341_Study

- Orange Pi 5
- Orangepi5_1.1.6_ubuntu_jammy_server_linux5.10.110

# Setup
~~~
sudo apt-get update
sudo apt-get install -y python3 git python3-pip
sudo apt-get install libgpiod2 python3-libgpiod
sudo apt-get install -y python3-smbus python3-dev i2c-tools
sudo pip3 install gpiod
sudo pip3 install adafruit-blinka
sudo pip3 install pillow
sudo pip3 install adafruit-circuitpython-rgb-display

orangepi@orangepi5:~$ sudo ln -s /dev/spidev4.1 /dev/spidev4.0
orangepi@orangepi5:~$ ls -al /dev/spi*
lrwxrwxrwx 1 root root     14 Oct 29 13:25 /dev/spidev4.0 -> /dev/spidev4.1
crw------- 1 root root 153, 0 Oct 29 13:23 /dev/spidev4.1
~~~

# Run
~~~
sudo python3 blinkatest.py
~~~
