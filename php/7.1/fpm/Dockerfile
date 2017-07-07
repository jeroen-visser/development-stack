FROM jvisser/php71-cli

RUN export DEBIAN_FRONTEND=noninteractive \
    && apt-get update && apt-get -y --no-install-recommends install php7.1-fpm \
    && apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*

COPY overrides.conf /etc/php/7.1/fpm/pool.d/z-overrides.conf

COPY php-fpm-startup /usr/bin/php-fpm
CMD /usr/bin/php-fpm

EXPOSE 9000