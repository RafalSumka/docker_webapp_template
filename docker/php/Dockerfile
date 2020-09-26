FROM php:7.3-fpm

COPY conf.d/php.ini /usr/local/etc/php/conf.d/docker_php.ini

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

RUN apt-get update && apt-get install -y \
    zlib1g-dev \
    libpng-dev \
    libpq-dev \
    libmagickwand-dev \
    git \
    zip \
    procps \
    wget

WORKDIR /var/www
