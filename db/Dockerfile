#FROM ubuntu:latest
#RUN apt-get update 
#install postgresql with apt-get
#RUN apt-get install -y postgresql postgresql-contrib
#initialize the database 
#RUN service postgresql start &&\
    #sudo -u postgres psql -c "CREATE DATABASE words;" &&\
    #sudo -u postgres psql -c "CREATE USER words WITH PASSWORD 'words';" &&\
    #sudo -u postgres psql -c "GRANT ALL PRIVILEGES ON DATABASE words TO words;"




FROM postgres:alpine
COPY words.sql /docker-entrypoint-initdb.d/words.sql
ENV POSTGRES_HOST_AUTH_METHOD=trust
