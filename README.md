# Laravel API Template

Building your API with [Laravel](https://laravel.com/).

## Prerequisites

0. Install dependencies.
  - Install `docker`, it's used for development.
  - Install PHP and `composer` on your machine, this is optional since you can ssh into the docker container and run PHP and `composer` there instead.
1. Replace all `laravel-api` in `docker-compose.yml` with your custom app name (in snake-case).
2. Copy `.env.example` to `.env`..
3. Replace `Laravel API` in `.env` with your app name.
4. Update `DB_DATABASE` in `.env` with a desired database name.

## Run it locally

```bash
# Run this on your machine if you have PHP/composer installed
# Otherwise you should run it inside your docker container
composer install

# Run this on your machine
docker-compose up -d
```

Then open `http://localhost:8080`

## Adding API Routes

Adding routes directly to `routes/api.php`, we have removed the `/api` prefix for you.

## Run Commands inside the Docker Container

```bash
docker exec -it <container_name> /bin/bash
```
