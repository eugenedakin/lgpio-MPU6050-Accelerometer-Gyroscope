# lgpio-MPU6050-Accelerometer-Gyroscope
Uses the Raspberry Pi 5, Xojo, and MPU6050 to detect tilt and other movements

If you've ever wanted to use your Raspberry Pi to detect tilt and other movements, Eugene is here showing how to connect a gyroscope and accelerometer sensor and read the results with Xojo. 
![](https://github.com/eugenedakin/lgpio-MPU6050-Accelerometer-Gyroscope/blob/main/Fritzing.png)

Ensure I2C is enabled on the Raspberry Pi. 

Install instructions are:

sudo apt install swig python-dev python3-dev
sudo apt install python-setuptools python3-setuptools
wget http://abyz.me.uk/lg/lg.zip
unzip lg.zip
cd lg
make
sudo make install
create a Light example program and copy the program and libraries to the RaspberryPi Desktop
give the executable permission to run with something like: 'sudo chmod +x Light'
run the program with something like: 'sudo ./Light'

