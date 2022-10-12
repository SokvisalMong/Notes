## Things to install

### docker-compose



### php 7.4

Add repository

`sudo add-apt-repository ppa:ondrej/php`

Install PHP and dependencies

`sudo apt-get install php7.4-cli php7.4-fpm php7.4-curl php7.4-gd php7.4-mysql php7.4-mbstring zip unzip`

### apache2

`sudo apt install apache2`

### mysql 8

`sudo apt install mysql-server`

### composer



### laravel 8

Comes with composer

### tailwind

https://tailwindcss.com/docs/installation

## Useful things

### Update and Upgrade

`sudo apt update && sudo apt upgrade`

### Check ports

`netstat -tlnp`

### Check if *blank* is running

`sudo service *blank* status`

Example:

`sudo service apache2 status`

### Start it

`sudo service *blank* start`

Example:

`sudo service mysql start`