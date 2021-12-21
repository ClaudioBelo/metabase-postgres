---
author: Claudio Belo Rodrigues Junior
email: claudiobelorjr@gmail.com
---
# metabase-postgresql

[README (pt-br)](./docs/readme-pt-br.md)

---

Repository to start an environment with [Metabase](https://www.metabase.com/) and [PostgreSQL](https://www.postgresql.org/).

## Services

for the environment it will be necessary to use the [Metabase](https://hub.docker.com/r/metabase/metabase) and [PostgreSQL](https://hub.docker.com/_/postgres) docker with the help of [docker compose](https://docs.docker.com/compose/).


These services are organized in the [docker-compose.yml](docker-compose.yml).

## Environment Variables

Environment variables can be found in the folder [config](./config).

[Metabase Environment](https://www.metabase.com/docs/latest/operations-guide/environment-variables.html):

- MB_DB_TYPE: Database type
- MB_DB_CONNECTION_URI: Database string connection.
- MB_ENCRYPTION_SECRET_KEY: Key for storing sensitive data.

[PostgreSQL](https://hub.docker.com/_/postgres):

- POSTGRES_DB: Database name.
- POSTGRES_USER: Database user.
- POSTGRES_PASSWORD: Database password.
