1) Install LAMP server on the Raspberry Pi 
   Refer : https://howtoraspberrypi.com/how-to-install-web-server-raspberry-pi-lamp/ 
   shell > cd /var/www/html
   shell > sudo rm *
   Put all the php files in this directory 

2) Set username : root and password : root to phpmyadmin and mysql
   You can use phpmyadmin from the web browser on the pi through http://localhost/phpmyadmin

3) Create database : IOT with table1 : count_all and table2 : user_login and attributes as shown in the phpmyadmin images 
   in the count_all and login folder respectively for master and
   Create database : IOT with table1 : counter2 and table2 : logger and attributes as shown in the phpmyadmin images 
   in the slave folder for slave

4) Put all the python code in the root directory with name button_debounce.py as shown in the images for slave 
   and master_code.py for master pi
   To run the python code in slave :
   shell > python button_debounce.py
   To run the python code in master :
   shell > python master_code.py

5) For Slave :
   shell > cd /var/www/html
   Put all the php files as there in the slave/api_php folder
   For Master :
   shell > cd /var/www/html
   shell > mkdir master_files
   shell > cd master_files
   Put all the files in the master/login/login_files folder in this directory.

6) For Slave : Put python code in the slave/button_code_python folder in the root directory
   For Master : Put python code in the master/count_all folder in the root directory.