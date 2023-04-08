# DBs

## requirements:
- docker

## run:
_assuming Docker is running_
```
cd ./postgres

docker build -t postgres-tfo-db .

docker run -d --name postgres-tfo -p 5432:5432 postgres-tfo-db
```