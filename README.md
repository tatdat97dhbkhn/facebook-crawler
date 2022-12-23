The facebook-crawler is built on the top of [Rails](https://rubyonrails.org/).

- [Requirements](#requirements)
- [Setup](#setup)
- [Start server in dev mode](#start-server-in-dev-mode)
- [Access Website](#access-website)
- [Env variables](#env-variables)
- [Database migrations](./doc/database-migrations.md)

## Requirements

- Docker (https://www.docker.com/)

## Setup
- `echo "fbc3e3eb4bd90f9e891b3a3bb169776e" > config/master.key`
- `chmod +x entrypoint_development.sh`
- `cp .env.example .env`
- `make build`
- `make db-setup`

## Start server in dev mode
- `make dev && make debug`

## Access Website
- http://localhost:3002/

## Env variables
- `PG_HOST` - specify Database host
- `PG_PORT` - specify Database port
- `PG_USER` - specify Database user
- `PG_PASSWORD` - specify Database user password
