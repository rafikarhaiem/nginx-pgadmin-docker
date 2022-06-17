FROM php:7.4-fpm

WORKDIR /var/www/html/code2

RUN groupadd -g 1000 www
RUN useradd -u 1000 -ms /bin/bash -g www www

COPY --chown=www:www . /var/www/html/code2

USER www
EXPOSE 9000
CMD ["php-fpm"]
