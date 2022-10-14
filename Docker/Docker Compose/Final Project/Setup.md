# Setting up our working Environment

## Prerequisites

Prerequisites:
- Running Ubuntu through WSL2 on Windows, Straight up Ubuntu, or MacOS
- Docker Desktop is installed
- Basic knowledge of linux things
- Make sure Docker is running in the background
- This extension on VSCode: `ms-vscode-remote.vscode-remote-extensionpack`

## Setting up Ubuntu WSL2 on Windows

fucking look it up yourself

After setting up an Ubuntu Distro on Windows

Make sure the close the distro

`exit`

Turn on these options

![if this shows up, you're fucked](Screenshot_832.png "Screenshot")

Save and restart Docker Desktop

Launch the Ubuntu Distro

Bada bing Bada boom

## Setting up Laravel Sail

First of all, find a snug comfy place for your project to rest

`mkdir ProjectFolder`

Go into said folder

`cd ProjectFolder`

Download the Docker Compose image

`curl -s "https://laravel.build/finalproject" | bash`

If the output is

`Docker is not running`

You go back and check things over dumb dumb

Aight, all good? All set? Lets go

Go into the project folder

`cd finalproject`

Makes your life easier

`alias sail='[ -f sail ] && sh sail || sh vendor/bin/sail'`

Build the server for the first time

`sail up`

After the terminal calms the fuck down

`sail down` or `Ctrl+C` that shit if you can't

To connect to the page, go to `localhost`

To open the file directory on VS Code

`code .`