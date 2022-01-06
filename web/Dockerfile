FROM php:apache
LABEL maintainer="Luka Todua"

#WORKDIR /web

RUN docker-php-ext-install mysqli
RUN apt-get update && apt-get -y upgrade
RUN apt-get install -y wget && apt-get clean
RUN apt-get install -y default-mysql-client

COPY . .

#RUN chmod +x setup.sh
#RUN bash setup.sh

RUN chown -R www-data:www-data wordpress
