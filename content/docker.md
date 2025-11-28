# Docker Setup

This project runs using:

- Laravel 12 (php:8.3-fpm)
- MySQL 8
- phpMyAdmin
- Composer installed in the container

## Start all containers

```
docker-compose up -d
```

## Rebuild app container

```
docker-compose build --no-cache
```

## Stop everything

```
docker-compose down
```
