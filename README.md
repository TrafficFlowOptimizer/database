# TrafficFlowOptimizer - moduł Baza Danych

## Opis:
Moduł odpowiedzialny jest za uruchomienie i dostęp do bazy danych.

## Jak uruchomić moduł

##### Wymagania:
* zainstalowany Docker
* zainstalowane narzędzie Docker Compose

##### Instrukcja:
* uruchomić Dockera
* w katalogu projektu: `docker compose up`

## Zarządzanie
Do bazy można podłączyć się bezpośrednio wykorzystując terminal lub [MongoDB Compass](https://www.mongodb.com/products/tools/compass). Aby zmienić nazwę użytkownika lub hasło należy edytować pola `MONGO_INITDB_ROOT_USERNAME` lub `MONGO_INITDB_ROOT_PASSWORD` w pliku konfiguracyjnym [compose](docker-compose.yaml).

### Dostęp za pomocą terminala
Po uruchomieniu bazy danych należy wpisać komendy:
```
docker exec -it mongodb bash
mongosh -u mongo -p mongo
```

### Dostęp za pomocą Compassa:
Po uruchomieniu bazy danych w Compassie należy:
* wybrać opcję `connect`
* wpisać URI `mongodb://localhost:27017`
* w `Advanced Connection Options/Authentication` należy wybrać metodę `Username/Password` i podać nazwę użytkownika `mongo` i hasło `mongo`

## Dokumentacja
* [Dokumentacja Mongo](https://www.mongodb.com/docs/)
* [Dokumentacja Dockera](https://docs.docker.com)
