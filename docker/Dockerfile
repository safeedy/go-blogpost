FROM php:7.2-fpm
MAINTAINER Safeedy <ambinintsoa.fs@gmail.com>

RUN apt-get update && apt-get install -y \
    apt-utils \
    ssh \
    vim \
    wget \
    rsync \
    git

# Install composer
RUN curl -sS https://getcomposer.org/installer | php && mv composer.phar /usr/local/bin/composer

USER project
WORKDIR /project