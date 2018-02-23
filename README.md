# Project docker-postgres

Dockerised PostgreSQL for local development database. 

# Requirements

Requires [docker-compose](https://docs.docker.com/compose/install).

# Configuration and Usage

First, set credentials using environment variables. Copy the file `etc/postgres.env.example` to `etc/postgres.env` and edit the values, at least `POSTGRES_PASSWORD`. 

Before starting the database you can set the environment variables `POSTGRES_VERSION` (default 10.0) and `POSTGRES_LOCAL_PORT` (default 5432) to control the database version and the mapped port on localhost.

Use `bin/up.sh` to start the database and `bin/down.sh` to stop the database. The data is persisted in a named volume.
