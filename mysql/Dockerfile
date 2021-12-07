FROM mysql

COPY ./initsql.sql /docker-entrypoint-initdb.d

ENV MYSQL_ROOT_PASSWORD=root

EXPOSE 3306

