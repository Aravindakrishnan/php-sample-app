FROM php:7.4-apache
RUN apt-get update
RUN apt-get install -y wget vim zip unzip libzip-dev libpng-dev
RUN docker-php-ext-install -j$(nproc) mysqli pdo_mysql gd zip pcntl exif
RUN a2enmod headers expires rewrite
WORKDIR /var/www/html
COPY . .
EXPOSE 80

