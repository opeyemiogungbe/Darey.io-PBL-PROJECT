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
