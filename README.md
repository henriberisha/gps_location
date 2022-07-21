# gps_location
This python script retrieves the GPS location from a USB GPS receiver

USB GPS receiver: GLOBAL SAT BU-353S4 Cable GPS with USB interface (SiRF Star IV)
https://www.globalsat.com.tw/en/a4-10593/BU-353S4.html
Note: It may work with other GPS USB receivers as well

The script works for LINUX OS
To make it work for WINDOWS, change port argument to a serial COM port
For example:  ser = serial.Serial(port='/dev/ttyUSB0', baudrate = 4800)   change to  ser = serial.Serial(port='COM5', baudrate = 4800)
NOTE: COM5 chosen for this example but it could be any number determined by your machine. Make sure you have the right serial port number o/w will not work

Dependencies:
1. Install python from: https://www.python.org/downloads/
2. Install pip: https://pip.pypa.io/en/stable/installation/
3. Install pyserial module in order to import the serial library: https://pypi.org/project/pyserial/
  -> In command line type: pip install pyserial

How to run:
In command line: python gps.py
