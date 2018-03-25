FROM php:7.2.3-apache-stretch

RUN apt-get update && \
        apt-get install -y --no-install-recommends \
        curl \
        sudo \
        wget \
        apt-transport-https \
        lsb-release \
        ca-certificates \
        git

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
        memcached \
		zip \
		unzip


# Install composer
RUN curl -sS https://getcomposer.org/installer | php
RUN mv composer.phar /usr/local/bin/composer