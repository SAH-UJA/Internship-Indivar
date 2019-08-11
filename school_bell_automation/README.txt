1) Install LAMP server on the Raspberry Pi 
   Refer : https://howtoraspberrypi.com/how-to-install-web-server-raspberry-pi-lamp/ 
   shell > cd /var/www/html
   shell > sudo rm *
   Put all the php files in this directory   

2) Set username : root and password : root to phpmyadmin and mysql
   You can use phpmyadmin from the web browser on the pi through http://localhost/phpmyadmin

3) Create database : school with table :classs and attributes as shown in the database.png image

4) Put all the python code in the root directory with name lcd.py as shown in the images
   To run the python code for lcd :
   shell > python lcd.py

5) Install indivar.apk in the Android Phone or open the indivar.aia file and go to blocks
   and edit the ip address in http://192.168.10.113/insert.php?   
                              http://192.168.10.113/delete.php?
			      http://192.168.10.113/update.php?
			      http://192.168.10.113/specific.php? with the ip address of the raspberry pi

6) Build the App from MITAppInventor and install the apk file generated

7) Use this app to alter the database and set the schedule of the class where the system is installed

8) Refer https://www.raspberrypi-spy.co.uk/2012/08/20x4-lcd-module-control-using-python/ for lcd circuitry and 
   https://iotguider.in/raspberrypi/learn-interfacing-ds3231-real-time-clock-raspberry-pi/ for RTC interfacing

9) Connect a Buzzer at pin 40 of the pi or as mentioned in the python code

	