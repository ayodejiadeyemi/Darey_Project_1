# Documentation of Project 1



## Web statck Implementation 

### Step 1 Installing apache

#### update a list of packages in package manager

`sudo apt update`
![Sudo Update](./Images/sudo_apt_update.png)

#### run apache2 package installation

`sudo apt install apache2`
![install apache2](./Images/install apache2.png)

#### Verify Apache2

`sudo systemctl status apache2`
![Verify apache2](./image/Verify apache2.png)
[Apache webpage](http://3.91.233.98/)

## Step 2
### Installing mysql

`sudo apt install mysql-server`
`sudo mysql`
`sudo mysql_secure_installation`
`sudo mysql -p`
![mysql verify](mysql verify page.png)

## step_3
### installing php

Step 3 Installing PHP.
`sudo apt install php libapache2-mod-php php-mysql`
`php -v`
![confirm php](./image/confirm php.png)

## step_4

Step 4 Creating a Virtual Host for your Website using Apache

`sudo mkdir /var/www/projectlamp`
`sudo chown -R $ubuntu:$ubuntu /var/www/projectlamp`
`sudo vi /etc/apache2/sites-available/projectlamp.conf`
`sudo ls /etc/apache2/sites-available`
`sudo a2ensite projectlamp`
`sudo a2dissite 000-default`
`sudo apache2ctl configtest`
`sudo systemctl reload apache2`
`code`

![alt text](image.jpg)
