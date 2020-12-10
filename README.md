# car_parking_project

Hello!
Welcome to my repo of automated car parking project.
Basically this project is designed for residential use. But it can be implemented to bigger projects also.
The necessary circuit diagram and codes are available here. To make the code run, 
-You need and Arduino IDE.
-You need to install Serial drivers
-Open the sketch and compile or verify.

For more info please visit : https://www.arduino.cc/en/software/

For linux users:

GUI:

-Download the necessary .tar.gz file

-Extract the zip and install the .deb file

Command Line:

-Extract the package

-cd to Arduino folder

-Install the bash script by typing ./install.sh

Please Read...

It might happen that when you upload a sketch - after you have selected your board and the serial port -, you get an error Error opening serial port ...

If you get this error, you need to set serial port permission.

Open Terminal and type:

ls -l /dev/ttyACM*

you will get something like:

crw-rw---- 1 root dialout 188, 0 5 apr 23.01 ttyACM0

The "0" at the end of ACM might be a different number, or multiple entries might be returned. The data we need is "dialout" (is the group owner of the file).

Now we just need to add our user to the group:

sudo usermod -a -G dialout <username>

where <username> is your Linux user name. You will need to log out and log in again for this change to take effect.


Thank you.
Have a great day
