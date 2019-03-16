FROM php:5.6-apache

RUN apt update -y && apt install libpng-dev -y

RUN docker-php-ext-install mysql mysqli gd pdo_mysql pdo

RUN curl -O https://pecl.php.net/get/xdebug-2.5.5.tgz && \
    pecl install xdebug-2.5.5.tgz && rm -rf xdebug-2.5.5.tgz

RUN docker-php-ext-enable xdebug
RUN a2enmod rewrite