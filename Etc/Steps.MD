# What is this for?

For my group mates who setup WSL2 on Windows and using Ubuntu 20.04.

This will make sure that everyone is on the same environment.

## Installing PHP

`sudo apt install software-properties-common ca-certificates lsb-release apt-transport-https -y`

`LC_ALL=C.UTF-8 add-apt-repository ppa:ondrej/php`

`sudo apt-get update && sudo apt-get upgrade`

`sudo apt install php7.4 -y`

`sudo apt-get install php-fpm php-mysql php7.4-cli php7.4-curl php7.4-mbstring php7.4-xml php7.4-zip php7.4-intl curl git unzip php-cli -y`

## Composer

`sudo apt update`

`cd ~`

`curl -sS https://getcomposer.org/installer -o /tmp/composer-setup.php`

`` HASH=`curl -sS https://composer.github.io/installer.sig` ``

`php -r "if (hash_file('SHA384', '/tmp/composer-setup.php') === '$HASH') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"`

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

## Installing NeoVim

`sudo add-apt-repository ppa:neovim-ppa/unstable`

`sudo apt-get update`

`sudo apt-get install neovim -y`