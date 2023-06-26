# Darey.io-PBL-PROJECT 1
## WEB STACK IMPLEMENTATION (LAMP STACK) IN AWS
A web stack is the collection of software (Built on each other) used for web development that comprises, at a minimum, an operating system (linux), a programming language(Php), database software(MySql) and a web server(Apache). Preparing our LAMP STACK will require us setting up our Apache2 webserver, MySql to store our database and Php to for display to the endusers of our web browser.

### UPDATING AND INSTALLING OUR APACHE2 WEBSERVER AND UPDATING THE FIREWALL
Apache is an open-source Web server, is is responsible for accepting directory (HTTP) requests from Internet users and sending them their desired information in the form of files and Web pages. it has a safe and secure file-sharing feature, allowing users to put files into the root directory of their Apache software and share them with other users.

** STEP 1**

Update our Operating system and install our apache2 webserver ruuning the following command:

`for updating our operating system run:
Sudo apt update` ![Screenshot 2023-06-21 052934](https://github.com/opeyemiogungbe/Darey.io-PBL-PROJECT/assets/136735745/32a7ca0e-3ffe-4fd4-85a6-540d23a7957f)




`for installing apache2 run: 
Sudo apt install apache2` To verify that apache2 is running as a Service in our OS, use following command` sudo systemctl status apache2`
![Screenshot 2023-06-21 053318](https://github.com/opeyemiogungbe/Darey.io-PBL-PROJECT/assets/136735745/7feff130-55f1-47fe-8ed7-e3cc2f877021)

Now that our Apache2 is running we will go ahead and set up MySql for our web database.


## INSTALLING MYSQL

MySQL is an open source relational database management system (RDBMS) with a client-server model. it's a software or service used to create and manage databases based on a relational level. Now we are going to run some commands to install and set up MySql. 

First we run `$: sudo apt install mysql-server` 
![Screenshot 2023-06-21 063232](https://github.com/opeyemiogungbe/Darey.io-PBL-PROJECT/assets/136735745/cd8898cd-be10-4bec-ab7e-f65c3bc052dc)

then we log into the MySql server to know we get the desired result running the command `$ sudo mysql`
![Screenshot 2023-06-21 063352](https://github.com/opeyemiogungbe/Darey.io-PBL-PROJECT/assets/136735745/460f21eb-240b-4595-9bc5-4d57101dd6f8)


We are also going to set up a password for the root user, using mysql_native_password as default authentication method by running the command `$ ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'PassWord.1'; ` before starting interactive script by running: `$ sudo mysql_secure_installation`. 

  After setting up our MySql password we are going to check if we can log into our console by running the command 

 ` $ sudo mysql -p` we should get a result like our image below: 
