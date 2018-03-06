# Docker Zammad

Docker image for the [Zammad](https://zammad.org) open source helpdesk/customer support system without ElasticSearch. This will use less RAM.

Inspired by the [official images](https://github.com/zammad/zammad-docker-compose).

Based on [ComputerScienceHouse's Image](https://github.com/ComputerScienceHouse/zammad-docker)

Both postgreSQL and MySQL are supported (included docker-compose file is ready for MySQL)

## Usage

#### docker-compose

Simply create `docker-compose.yml` filling it with a random password for MySQL/mariaDB database.

#### Env Variables

As per [ComputerScienceHouse's Image](https://github.com/ComputerScienceHouse/zammad-docker):

The `zammad` container can be configured with the following environment variables:

| Variable      | Description                                                          | Required |
|---------------|----------------------------------------------------------------------|----------|
| `DB_ADAPTER`  | Database adapter to use (options: `postgresql`, `mysql2`)            | Yes      |
| `DB_HOSTNAME` | Hostname of the database container or server                         | Yes      |
| `DB_PORT`     | Port of the database server (defaults to the adapter's default port) | No       |
| `DB_NAME`     | Name of the database                                                 | Yes      |
| `DB_USERNAME` | Username for the database user                                       | Yes      |
| `DB_PASSWORD` | Password for the database user                                       | No       |

