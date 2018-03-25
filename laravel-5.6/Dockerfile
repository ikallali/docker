FROM php:7.2.3-apache-stretch

RUN apt-get update && \
        apt-get install -y --no-install-recommends \
        curl \
        wget \
        apt-transport-https \
        lsb-release \
        ca-certificates \
        git

RUN wget -O /etc/apt/trusted.gpg.d/php.gpg https://packages.sury.org/php/apt.gpg && /bin/sh -c 'echo "deb https://packages.sury.org/php/ $(lsb_release -sc) main" > /etc/apt/sources.list.d/php.list'
RUN curl -sL https://deb.nodesource.com/setup_8.x | bash -

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