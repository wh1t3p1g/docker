FROM php:5.6-apache

RUN apt update -y && apt install libpng-dev -y

RUN docker-php-ext-install mysql mysqli gd pdo_mysql pdo
RUN a2enmod rewrite