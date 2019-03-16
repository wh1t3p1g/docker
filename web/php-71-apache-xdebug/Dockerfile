FROM 0kami/env:php71-apache

RUN echo "xdebug.remote_enable=on" >> /usr/local/etc/php/php.ini && \
    echo "xdebug.auto_trace=on" >> /usr/local/etc/php/php.ini && \
    echo "xdebug.remote_log = /tmp/xdebug.log" >> /usr/local/etc/php/php.ini && \
    echo 'xdebug.remote_handler = dbgp' >> /usr/local/etc/php/php.ini && \
    echo "xdebug.idekey=PHPSTORM" >> /usr/local/etc/php/php.ini && \
    echo "xdebug.remote_host=10.254.254.254" >> /usr/local/etc/php/php.ini && \
    echo "xdebug.remote_post=9000" >> /usr/local/etc/php/php.ini