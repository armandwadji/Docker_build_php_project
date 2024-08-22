#FROM php:8.2-apache
#RUN docker-php-ext-install mysqli
#COPY . /usr/src/myapp
#WORKDIR /usr/src/myapp
#CMD [ "php", "./index.php" ]

#FROM php:5.6-apache
#
## INSTALL DEPENDDENCIES
#RUN docker-php-ext-install mysqli
#
## PHP
#RUN apt-get update && apt-get upgrade
#RUN apt-get install -y zlib1g-dev libwebp-dev libpng-dev && docker-php-ext-install gd
#RUN apt-get install libzip-dev -y && docker-php-ext-install zip
#
## Apache
#RUN a2enmod rewrite
#RUN service apache2 restart
#
#EXPOSE 80

FROM php:5.6-apache

RUN docker-php-ext-install mysqli

WORKDIR /var/www/html
COPY ./src ./
