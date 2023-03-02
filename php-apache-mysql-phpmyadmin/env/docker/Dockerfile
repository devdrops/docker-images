FROM php:7-apache

LABEL maintainer="Davi Marcondes Moreira <davi.marcondes.moreira@gmail.com>"

RUN a2enmod rewrite && \
    apt-get update && apt-get install -y git libpng-dev libjpeg-dev zip unzip \
    && docker-php-ext-configure gd --with-jpeg=/usr \
    && docker-php-ext-install gd \
    && rm -rf /var/lib/apt/lists/* \
    && docker-php-ext-install mysqli

VOLUME /var/www/html

CMD ["apache2-foreground"]
