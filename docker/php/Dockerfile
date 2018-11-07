FROM php:7.2-fpm

COPY conf.d/php.ini /usr/local/etc/php/conf.d/docker_php.ini

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

WORKDIR /var/www
