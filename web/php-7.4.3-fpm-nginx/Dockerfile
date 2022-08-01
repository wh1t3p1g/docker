FROM php:7.4.3-fpm

RUN docker-php-ext-install -j$(nproc) opcache

RUN mkdir /tmp/opcache && chmod -R 777 /tmp/opcache 
COPY php.ini /usr/local/etc/php/php.ini