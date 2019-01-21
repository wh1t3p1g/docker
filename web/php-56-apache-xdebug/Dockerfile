FROM php:5.6-apache

RUN apt update -y && apt install libpng-dev -y

RUN docker-php-ext-install mysql mysqli gd pdo_mysql
RUN pecl install xdebug-2.5.5
RUN docker-php-ext-enable xdebug 
RUN docker-php-ext-install pdo

RUN echo "xdebug.remote_enable=1" >> /usr/local/etc/php/php.ini && \
    echo "xdebug.auto_trace=on" >> /usr/local/etc/php/php.ini && \
    echo "xdebug.trace_output_dir='/tmp/'" >> /usr/local/etc/php/php.ini && \
    echo 'xdebug.collect_params=4' >> /usr/local/etc/php/php.ini && \
    echo 'xdebug.remote_autostart=1' >>  /usr/local/etc/php/php.ini && \
    echo "xdebug.remote_connect_back=0" >> /usr/local/etc/php/php.ini && \
    echo 'xdebug.remote_host=10.254.254.254' >>   /usr/local/etc/php/php.ini && \
    echo "xdebug.max_nesting_level=250" >> /usr/local/etc/php/php.ini && \
    echo "xdebug.collect_return=on" >> /usr/local/etc/php/php.ini && \
    echo "xdebug.idekey=PHPSTORM" >> /usr/local/etc/php/php.ini && \
    echo "xdebug.remote_post=9000" >> /usr/local/etc/php/php.ini 