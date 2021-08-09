
# Let's build a forum with TDD

In this project i will show how to build a project with TDD


## Installation

Install the project

For fresh installation

```bash
  mkdir src
  cd src
   docker-compose run --rm composer create-project --prefer-dist laravel/laravel .
```
if you clone the project then run

```bash
   docker-compose run --rm composer update
   docker-compose run --rm composer dump-autoload
   docker-compose run --rm php php artisan key:generate
   docker-compose run --rm php php artisan migrate:fresh
   sudo chmod -R 777 src/storage
```
    
## Run Locally

For the first time run and build the docker

```bash
  docker-compose up -d --build server
```

Start the server

```bash
   docker-compose up -d server
```

Terminate the server

```bash
   docker-compose down server
```

## Running Tests

Mysql bash

```bash
   docker-compose exec mysql /bin/bash
```

PHP bash

```bash
    docker-compose exec php /bin/sh
```