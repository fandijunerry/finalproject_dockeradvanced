FROM php:7.2-apache
LABEL maintainer <fandi.junerry@gmail.com>
COPY file-web /var/www/html
HEALTHCHECK --interval=10s --timeout=2s --retries=3 CMD curl -f http://localhost || exit 1
RUN docker-php-ext-install pdo pdo_mysql
#RUN docker-php-ext-install mysqli pdo pdo_mysql