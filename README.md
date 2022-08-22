# Blog MongoDB configuration deployment description

## Start local database environment with mongodb docker image

- Create the environment file `.env`
- Setup the environment variables into the `.env` file
    - `DB_DATA_PATH=/home/data-mongodb`: place where you are going to save the mondodb data
    - `DB_PORT=27017`: database port
- Start docker image
    - `docker network create blogdb`
    - `docker-compose -f docker-compose.local.yml up -d`

## Backups

**List of backups actions**

`docker exec tutum-backup ls /backup`

**Restore from backup**

`docker exec tutum-backup /restore.sh /backup/2015.08.06.171901`

## Constributions

All contributions are welcome
