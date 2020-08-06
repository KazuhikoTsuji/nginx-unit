# keep our base image as small as possible
FROM nginx/unit:1.18.0-php7.3

# port used by the listener in config.json
EXPOSE 80

# application setup
RUN apt update && apt install -y \
    software-properties-common \
    php7.3-dom \
    php7.3-gd \
    php7.3-mysql \
    php7.3-mbstring \
    && apt clean \
    && rm -rf /var/lib/apt/lists/*
RUN mkdir /www/  
COPY ./drupal-8.6.4/ /www/
COPY ./config.json /docker-entrypoint.d/config.json
