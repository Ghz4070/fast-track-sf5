FROM php:8.0.1-fpm-alpine3.13

RUN set -ex \
  && apk --no-cache add \
  postgresql-dev

RUN docker-php-ext-install pdo pdo_pgsql

WORKDIR /var/www/html

CMD php-fpm

EXPOSE 9000
