FROM mariadb
LABEL maintainer="Luka Todua"

ENV MYSQL_ROOT_PASSWORD=pw123
ENV MYSQL_DATABASE=wordpress

RUN apt-get update && apt-get -y upgrade && apt-get clean
RUN apt-get install -y mysql-client-8.0 && apt-get install -y default-mysql-client
