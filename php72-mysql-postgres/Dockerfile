FROM php:7.2-alpine

WORKDIR /app

COPY . .

ENTRYPOINT /bin/sh

RUN apk update           \
    apk add --no-cache    \
    gmp                  \
    imagemagick


# Install composer
ENV COMPOSER_HOME /composer
ENV PATH ./vendor/bin:/composer/vendor/bin:$PATH
ENV COMPOSER_ALLOW_SUPERUSER 1
RUN curl -s https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin/ --filename=composer

# Install PHP_CodeSniffer
RUN composer global require "squizlabs/php_codesniffer=*"
