FROM php:7.3-apache

RUN apt update -y && apt install libpng-dev -y

RUN docker-php-ext-install mysqli gd pdo_mysql pdo