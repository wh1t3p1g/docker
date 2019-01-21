FROM phpstorm/php-56-apache-xdebug-25

RUN echo "xdebug.auto_trace=on" >> /usr/local/etc/php/php.ini
RUN echo "xdebug.trace_output_dir='/tmp/'" >> /usr/local/etc/php/php.ini
RUN echo 'xdebug.collect_params=4' >> /usr/local/etc/php/php.ini

RUN echo "xdebug.remote_enable=1" >> /usr/local/etc/php/php.ini
RUN echo 'xdebug.remote_autostart=1' >>  /usr/local/etc/php/php.ini
RUN echo "xdebug.remote_connect_back=0" >> /usr/local/etc/php/php.ini
RUN echo 'xdebug.remote_host=docker.for.mac.localhost' >>   /usr/local/etc/php/php.ini
RUN echo "xdebug.max_nesting_level=250" >> /usr/local/etc/php/php.ini
RUN echo "xdebug.collect_return=on" > /usr/local/etc/php/php.ini