FROM jvisser/base

# Install dotdeb repo, PHP7, composer and selected extensions
RUN apt-get update \
    && apt-get -y --no-install-recommends install php7.0-cli php7.0-curl \
        php7.0-json php7.0-mcrypt php7.0-opcache php7.0-readline php7.0-xml php7.0-zip php-xdebug \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*

CMD ["php", "-a"]

# If you'd like to be able to use this container on a docker-compose environment as a quiescent PHP CLI container
# you can /bin/bash into, override CMD with the following - bear in mind that this will make docker-compose stop
# slow on such a container, docker-compose kill might do if you're in a hurry
# CMD ["tail", "-f", "/dev/null"]