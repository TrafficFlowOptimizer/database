# DBs

## requirements:
- docker

## run:
_assuming Docker is running_
```
docker compose up -d
```

## manage:
```
docker exec -it mongodb bash
mongosh -u mongo -p mongo
```