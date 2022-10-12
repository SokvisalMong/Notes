# What is this for?

For my group mates who setup WSL2 on Windows and using Ubuntu 20.04.

This will make sure that everyone is on the same environment.

## Installing PHP

`sudo apt install software-properties-common ca-certificates lsb-release apt-transport-https`

`LC_ALL=C.UTF-8 add-apt-repository ppa:ondrej/php`

`sudo apt-get update && sudo apt-get upgrade`

`sudo apt install php7.4`

`sudo apt-get install php-fpm php-mysql php7.4-cli php7.4-curl php7.4-mbstring php7.4-xml php7.4-zip php7.4-intl curl git unzip php-cli`

## Composer

`cd ~`

`curl -sS https://getcomposer.org/installer -o composer-setup.php`

`sudo php composer-setup.php –install-dir=/usr/local/bin –filename=composer`

## Apache 2

`sudo apt install apache2`

### Start Apache 2

`sudo service apache2 start`

## MySQL

`sudo apt install mysql-server`

### Start MySQL

`sudo service mysql start`

## Docker

`sudo apt update`

`sudo apt install apt-transport-https ca-certificates curl software-properties-common`

`curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -`

`sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"`

`apt-cache policy docker-ce`

`sudo apt install docker docker-ce`

`sudo apt install containerd`

### Start docker

`sudo service docker start`

## Docker Compose

Follow these [steps](https://docs.docker.com/engine/install/ubuntu/#set-up-the-repository)

## Installing NeoVim

`sudo add-apt-repository ppa:neovim-ppa/unstable`

`sudo apt-get update`

`sudo apt-get install neovim`