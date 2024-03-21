# Blog MySQL configuration deployment description

## Start local database environment with mysql docker image

- Create the environment file `.env`
- Setting up the environment variables into the `.env` file
    - `DB_DATA_PATH=/home/data-mongodb`: place where you are going to save the mysql data
    - `DB_PORT=3306`: database port
    - `TIMEZONE=Europe/Berlin`
- Start docker image
    - `docker network create blogdb`
    - `docker-compose -f docker-compose.local.yml up -d`

> Note: if you want to know your local timezone, execute the command: `cat /etc/timezone`

## Contributions

All contributions are welcome
