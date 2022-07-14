FROM php:8.1-apache
#build mysql and intl extensions
RUN apt-get -y update \
&& apt-get install -y libicu-dev \ 
&& docker-php-ext-configure intl \
&& docker-php-ext-install pdo_mysql \ 
&& docker-php-ext-install intl
#dont think this is needed
RUN a2enmod rewrite