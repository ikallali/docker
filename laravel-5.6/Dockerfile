FROM php:7.2.3-apache-stretch

RUN apt-get update && \
        apt-get install -y --no-install-recommends \
        curl \
        sudo \
        wget \
        apt-transport-https \
        lsb-release \
        ca-certificates \
        git \
        gnupg \
        dirmngr \
        software-properties-common
        

  

RUN add-apt-repository ppa:ondrej/php

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
        memcached \
		zip \
		unzip \
		php7.2-mysql \
		php7.2-xml \
		php7.2-gd \
		php7.2-mbstring \
		php7.2-curl \
		php7.2-soap \
		php7.2-zip \
		php7.2-sqlite3 \
		php-memcached


# Install composer
RUN curl -sS https://getcomposer.org/installer | php
RUN mv composer.phar /usr/local/bin/composer