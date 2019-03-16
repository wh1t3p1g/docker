FROM php:7.1-apache

RUN apt update -y && apt install -y libpng-dev libzip-dev libfreetype6-dev libjpeg62-turbo-dev libgd-dev

RUN docker-php-ext-install mysqli pdo_mysql pdo zip

RUN docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/  &&  \
    docker-php-ext-install gd

RUN curl -O https://pecl.php.net/get/xdebug-2.7.0.tgz && \
    pecl install xdebug-2.7.0.tgz && rm -rf xdebug-2.7.0.tgz
RUN docker-php-ext-enable xdebug

RUN a2enmod rewrite