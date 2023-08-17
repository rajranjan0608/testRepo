FROM postgres:latest

# copy schema and seed data dump
COPY data/* /docker-entrypoint-initdb.d/

ARG POSTGRES_USER=user
ARG POSTGRES_PASSWORD=password
ARG POSTGRES_DB=raj_db

ENV POSTGRES_USER=$POSTGRES_USER
ENV POSTGRES_PASSWORD=$POSTGRES_PASSWORD
ENV POSTGRES_DB=$POSTGRES_DB

EXPOSE 5432

CMD ["postgres"]

