PostgreSQL Monitoring
=====================

This repo provides PostgreSQL online monitoring setup based on Prometheus + postgres-exporter + Grafana.

Prerequisites
-------------

* Any Linux OS
* docker
* docker-compose v2

Configuration
-------------

# Edit `docker.env` file and specify connection string for your PostgreSQL
  instance. Note that since this connection string will be used to connect to
  Postgres from inside docker container, you have to use `host.docker.internal`
  as a host name if PostgreSQL is running on the same host where you are running
  docker-compose.
# Run containers by running `docker compose --env-file=docker.env up`.
# Open http://localhost:3000/ in your browser. Default Grafana's user and password are admin / admin.

