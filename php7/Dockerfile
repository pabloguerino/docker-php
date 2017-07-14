FROM alpine:edge
MAINTAINER Pablo Guerino <pablo.guerino@jadelabs.net>

WORKDIR /src

RUN addgroup www -S && adduser -D -S -G www www

RUN apk --upgrade --no-cache --repository http://dl-cdn.alpinelinux.org/alpine/edge/community  add \
    bash \
    ca-certificates \
    curl \
    unzip \
    php7 \
    php7-bcmath \
    php7-ctype \
    php7-curl \
    php7-dom \
    php7-fileinfo \
    php7-gd \
    php7-gettext \
    php7-iconv \
    php7-intl \
    php7-json \
    php7-mbstring \
    php7-mcrypt \
    php7-mysqlnd \
    php7-opcache \
    php7-openssl \
    php7-pdo \
    php7-pdo_mysql \
    php7-pdo_pgsql \
    php7-pdo_sqlite \
    php7-phar \
    php7-posix \
    php7-session \
    php7-soap \
    php7-tokenizer \
    php7-xml \
    php7-xmlreader \
    php7-xmlwriter \
    php7-zip \
    php7-zlib

COPY php.ini /etc/php7/php.ini

CMD ["php", "-a"]
