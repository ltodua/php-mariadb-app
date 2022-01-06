FROM mariadb
LABEL maintainer="Luka Todua"

RUN apt-get update && apt-get -y upgrade && apt-get clean
RUN apt-get install -y mysql-client-8.0 && apt-get install -y default-mysql-client