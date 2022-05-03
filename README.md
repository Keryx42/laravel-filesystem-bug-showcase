# Informations for the one who tries to fix this bug

This is a fresh laravel installation with following modifications
- config/filesystems.php
  - a ftp configuration was added pointing to some public ftp I looked up for showcasing. Any ftp server will do
- routes/web.php:18
  - a write action to the ftp is called. This causes the ErrorException (Bug)

## Created for the following bug report
https://github.com/laravel/framework/issues/42234

## Get it running
I used on my machine
- PHP 8.1.0
- Composer 2.1.14

### Clone this repo
`git@github.com:Keryx42/laravel-filesystem-bug-showcase.git`

### Install Composer dependencies
`composer install` 

### Start the server
Just run `php artisan serve`.
You will get the bug presented directly on the main page
