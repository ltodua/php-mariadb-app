FROM php:apache
LABEL maintainer="Luka Todua"

ENV MYSQL_ROOT_PASSWORD=pw123
ENV MYSQL_DATABASE=wordpress

RUN docker-php-ext-install mysqli
RUN apt-get update && apt-get -y upgrade 
RUN apt-get install -y wget && apt-get clean

RUN wget https://wordpress.org/wordpress-5.8.tar.gz && tar zxf wordpress-5.8.tar.gz
RUN echo "<?php header("Location: ./wordpress/"); ?>" > index.php

