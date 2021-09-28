FROM php:8.0-fpm

RUN apt-get update
RUN apt-get install -y git zip unzip libicu-dev

# add extension module
RUN docker-php-ext-install pdo_mysql intl

# install composer
COPY --from=composer:2.0.12 /usr/bin/composer /usr/bin/composer
