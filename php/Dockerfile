FROM php:7.3-apache

RUN chown www-data var/www/ -R

WORKDIR $APPLICATION_ROOT

RUN apt-get update && apt-get upgrade -y
RUN docker-php-ext-install mysqli
EXPOSE 80
