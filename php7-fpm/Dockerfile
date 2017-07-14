FROM jadelabs/php
MAINTAINER Pablo Guerino <pablo.guerino@jadelabs.net>

WORKDIR /src

RUN apk add --upgrade --no-cache --repository http://nl.alpinelinux.org/alpine/edge/community \
    php7-fpm

COPY php.ini /etc/php7/php.ini
COPY php-fpm.conf /etc/php7/php-fpm.conf

EXPOSE 9000
CMD ["php-fpm7", "-F"]
