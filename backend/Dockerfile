FROM php:7.4-fpm-alpine as backend-stage

LABEL maintainer="LuuSean"

RUN docker-php-ext-install pdo_mysql sockets
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

WORKDIR /var/www/html/backend
COPY . .