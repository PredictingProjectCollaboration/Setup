# Start MongoDB Service

In your MongoDB project folder (where `docker-compose.yml` and `.env` are located), run:

```bash
docker compose --env-file .env up -d
```

## Download MongoDB Compass

```bash
https://www.mongodb.com/try/download/shell

```

## Create connection in MongoDB Compass

Paste connection string when creating connection

```bash
mongodb://localhost:27017/?authSource=admin
```
