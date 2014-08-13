# Twilio Skeleton Application built on the Jolt framework

Use this skeleton application to quickly setup and start working on a new Twilio application. This application uses the latest Jolt and Twilio repositories.

This skeleton application was built for Composer. This makes setting up a new Twilio application quick and easy.

## Install Composer

If you have not installed Composer, do that now. I prefer to install Composer globally in `/usr/local/bin`, but you may also install Composer locally in your current working directory. For this tutorial, I assume you have installed Composer locally.

<http://getcomposer.org/doc/00-intro.md#installation>

## Install the Application

After you install Composer, run this command from the directory in which you want to install your new Jolt Framework application.

    php composer.phar create-project freekrai/jolt-skeleton [my-app-name]

Replace <code>[my-app-name]</code> with the desired directory name for your new application. You'll want to point your virtual host document root to your new application's directory.

Edit config.ini with your configuration settings, and that's it! Now go build something cool.

## Built-in server

With PHP 5.4 and up, we have a built-in web server, this is handy for local development.

You can run your new app locally using the following command in the terminal:

	php -S localhost:8888 server.php
	
This will route all processes through the server.php file, which whill then treat this the same as if it was on a web server. This lets you handle local development nicely.

## Structure

The Twilio Skeleton Application comes complete with a few pieces already in place.

1. SQLite database located in content/data/data.sqlite, this database holds user information as well as a call log. It also has a post table for doing whatever else you may want it to do.

2. Views, all output is handled by the views folder located in content/views/ the filenames correspond to actions used by the system.

3. User system, you can quickly set up a user system with the /signup, /login and /dashboard actions that are already set up. Once logged in, you will also see a user dashboard and the ability to manage other users.

You can keep these, or remove them at your leisure, I just fiind it easier to get going when you already have something to work with. 

Enjoy :)