FROM php:8.2.20-apache

RUN apt-get update && \
    apt-get install libonig-dev && \
    apt-get install -y libpq-dev && \
    docker-php-ext-install pdo_mysql mysqli mbstring

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

RUN apt-get install unzip

RUN a2enmod rewrite