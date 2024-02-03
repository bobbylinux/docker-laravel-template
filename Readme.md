# Docker Laravel Php 8.3.2 Nginx MariaDB Template

## Configure mysql data
add directory "mysql_data" under "database" directory.

## Download laravel app
```sh
git clone git@github.com:laravel/laravel.git app
```
## Build
```sh
docker-compose -f docker-compose.yml build
```
## Run
```sh
docker-compose -f docker-compose.yml build
```
## Install Laravel
```sh
 docker-compose exec php-fpm composer install
 docker-compose exec php-fpm php artisan key:generate
 docker-compose exec php-fpm php artisan config:cache
```