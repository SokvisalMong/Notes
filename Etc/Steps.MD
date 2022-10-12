# What is this for?

For my group mates who setup WSL2 on Windows and using Ubuntu 20.04.

Specifically for Laravel 8.

This will make sure that everyone is on the same environment.

## Zip/Unzip

`sudo apt update`

`sudo apt-get install zip unzip -y`

## Installing PHP

`sudo apt install software-properties-common ca-certificates lsb-release apt-transport-https -y`

`LC_ALL=C.UTF-8 add-apt-repository ppa:ondrej/php`

`sudo apt update`

`sudo apt install php7.4 -y`

`sudo apt install php7.4-mysql php7.4-mbstring php7.4-xml php7.4-curl -y`

`sudo apt install php7.4-common php7.4-bcmath openssl php7.4-json php7.4-mbstring -y`

`php -v`

## Composer

`sudo apt update`

`cd ~`

`curl -sS https://getcomposer.org/installer -o /tmp/composer-setup.php`

`` HASH=`curl -sS https://composer.github.io/installer.sig` ``

`php -r "if (hash_file('SHA384', '/tmp/composer-setup.php') === '$HASH') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"`

`sudo php /tmp/composer-setup.php --install-dir=/usr/local/bin --filename=composer`

## Apache 2

`sudo apt install apache2 -y`

### Start Apache 2

`sudo service apache2 start`

## MySQL

`sudo apt install mysql-server -y`

### Start MySQL

`sudo service mysql start`

## Docker Compose

Follow these [steps](https://docs.docker.com/engine/install/ubuntu/#set-up-the-repository)

## Docker

`sudo apt update`

`sudo apt install apt-transport-https ca-certificates curl software-properties-common -y`

`curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -`

`sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"`

`apt-cache policy docker-ce`

`sudo apt install docker docker-ce -y`

`sudo apt install containerd -y`

### Start docker

`sudo service docker start`

# Extra

## Installing NeoVim

`sudo add-apt-repository ppa:neovim-ppa/unstable`

`sudo apt-get update`

`sudo apt-get install neovim -y`