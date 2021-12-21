---
author: Claudio Belo Rodrigues Junior
email: claudiobelorjr@gmail.com
---
# metabase-postgresql

---

Este repositório tem como objetivo ser um passo inicial para a estruturação de um ambiente do [Metabase](https://www.metabase.com/) com um banco de dados [PostgreSQL](https://www.postgresql.org/).

## Serviços

Para a estruturação do ambiente serão utilizados o docker do [metabase](https://hub.docker.com/r/metabase/metabase) e o [PostgreSQL](https://hub.docker.com/_/postgres) com o auxilio da ferramenta [docker compose](https://docs.docker.com/compose/).

Esses serviços serão estão organizados no arquivo [docker-compose.yml](docker-compose.yml).

## Variáveis de Ambiente

As variavéis de ambiente podem ser encontradas na pasta [config](./config) e estão.

[Metabase](https://hub.docker.com/r/metabase/metabase):

- MB_DB_TYPE: Tipo de banco de dados.
- MB_DB_CONNECTION_URI: Texte de conexão com o PostgreSQL.
- MB_ENCRYPTION_SECRET_KEY: Chave para armazenamento de dados sensíveis.

[PostgreSQL](https://hub.docker.com/_/postgres):

- POSTGRES_DB: Banco de dados padrão.
- POSTGRES_USER: Usuário do banco de dados.
- POSTGRES_PASSWORD: Senha do banco de dados.
