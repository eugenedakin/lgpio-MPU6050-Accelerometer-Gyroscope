# lgpio-MPU6050-Accelerometer-Gyroscope
Uses the Raspberry Pi 5, Xojo, and MPU6050 to detect tilt and other movements. Prior Raspberry Pi SBC (Single Board Computers) can be used by modifying the lgGpiochipOpen command. 

If you've ever wanted to use your Raspberry Pi to detect tilt and other movements, Eugene is here showing how to connect a gyroscope and accelerometer sensor and read the results with Xojo. 
![](https://github.com/eugenedakin/lgpio-MPU6050-Accelerometer-Gyroscope/blob/main/Fritzing.png)

Ensure I2C is enabled on the Raspberry Pi. 

To use the lgpio with Raspberry Pi 4 or older systems, get the successful chip handle (not a zero) with the following command:
| Initialize the Raspberry Pi 4 lgpio |
| --------------------------------- |
| MyChipHandle = lgGpiochipOpen(0) //dev/gpiochip0 for Raspberry Pi 4 or older |

To use the lgpio with the Raspberry Pi 5 board, get the chip handle with the following command:
| Initialize the Raspberry Pi 5 lgpio |
| --------------------------------- |
| MyChipHandle = lgGpiochipOpen(4) //dev/gpiochip4 for Raspberry Pi 5 |

Install instructions are:

1. sudo apt install swig python-dev python3-dev
2. sudo apt install python-setuptools python3-setuptools
3. wget http://abyz.me.uk/lg/lg.zip
4. unzip lg.zip
5. cd lg
6. make
7. sudo make install
8. open the example program and copy the program and libraries to the RaspberryPi Desktop
9. give the executable permission to run with something like: 'sudo chmod +x MPU6050'
10. run the program with something like: 'sudo ./MPU6050'

Screen Grab of Running Program
![](https://github.com/eugenedakin/lgpio-MPU6050-Accelerometer-Gyroscope/blob/main/ScreenGrab-2.png)
