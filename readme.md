<h1 align="center">Laravel 5.6 CRUD app</h1>
<br>
<p align="center">
  <a href="https://laravel.com/">
    <img alt="Laravel" title="Laravel" src="https://cdn-images-1.medium.com/max/720/1*hUuioUcs_0tzu7mMwr9udA.png" width="310">
  </a>
</p>
<p align="center">
    <img src="https://img.shields.io/badge/laravel-v5.6-green.svg" />
    <img src="https://img.shields.io/badge/bootstrap-v4.0.0-green.svg" />
</p>

## Table of Contents

- [Introduction](#introduction)
- [Built With](#built-with)
- [Install](#install)

## Introduction

A Laravel 5.6 CRUD application, which showcases widley used CRUD features. Uses minimal bootstrap styling. Requires a MYSQL table to store data. 

## Built-With

- Laravel v5.6
- Bootstrap v4.0.0
- MySQL

## Install 

* Clone my Git <a href="https://github.com/maxsilvauk/laravel-crud.git">repository</a> into your htdocs.
```
git clone https://github.com/maxsilvauk/laravel-crud.git
```
* Move to the laravel root folder.
```
cd laravel_crud
```
* Install composer globally (You will need PHP installed).
```
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('SHA384', 'composer-setup.php') === '544e09ee996cdf60ece3804abc52599c22b1f40f4323403c44d44fdfdd586475ca9813a858088ffbc1f233e9b180f061') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"
```
* Move the composer and install dependances.
```
mv composer.phar /usr/local/bin/composer
composer install
```
* Create a .env file for Laravel
```
touch .woo && vi .woo i
```
* Type the following, once entered press ESC to exist insert mode then :x to save the file.
```
APP_NAME="Laravel CRUD"
APP_ENV=local
APP_KEY=base64:EslUg/T3QR6T0GnMbc4v9/lrAIgF8/KoQMs9z2t2x/s=
APP_DEBUG=true
APP_URL=http://localhost

LOG_CHANNEL=stack

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravel_crud
DB_USERNAME=YOUR_MYSQL_USERNAME
DB_PASSWORD=YOUR_MYSQL_PASS

BROADCAST_DRIVER=log
CACHE_DRIVER=file
SESSION_DRIVER=file
SESSION_LIFETIME=120
QUEUE_DRIVER=sync

REDIS_HOST=127.0.0.1
REDIS_PASSWORD=null
REDIS_PORT=6379

MAIL_DRIVER=smtp
MAIL_HOST=smtp.mailtrap.io
MAIL_PORT=2525
MAIL_USERNAME=null
MAIL_PASSWORD=null
MAIL_ENCRYPTION=null

PUSHER_APP_ID=
PUSHER_APP_KEY=
PUSHER_APP_SECRET=
PUSHER_APP_CLUSTER=mt1

MIX_PUSHER_APP_KEY="${PUSHER_APP_KEY}"
MIX_PUSHER_APP_CLUSTER="${PUSHER_APP_CLUSTER}"
```
* Create a MySQL database called 'laravel_crud' and migrate the tables.
```
php artisan migrate
```
* Run the development server.
```
php artisan serve
```
* Locate the application in the browser.
```
http://localhost:8000
```