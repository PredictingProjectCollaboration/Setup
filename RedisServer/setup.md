# Start Redis Service

In your Redis project folder (where `docker-compose.yml` and `.env` are located), run:

```bash
docker compose --env-file .env up -d
```

## Open the Redis CLI

```bash
docker exec -it redis-server redis-cli
```

## Authenticate and test

```bash
auth your_secure_password
set key1 "value"
get key1
```
