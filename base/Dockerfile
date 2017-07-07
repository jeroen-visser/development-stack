FROM ubuntu:xenial

# Fixes some weird terminal issues such as broken clear / CTRL+L
ENV TERM=linux

# Install cURL and vim
RUN apt-get update \
    && apt-get install -y --no-install-recommends curl ca-certificates vim \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*