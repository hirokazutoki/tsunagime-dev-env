## How to clone
```shell
$ git clone https://github.com/hirokazutoki/tsunagime-dev-env.git tsunagime
$ git clone https://github.com/hirokazutoki/tsunagime-api.git tsunagime/tsunagime-api
```

## How to start
```shell
$ cd tsunagime
$ cp .env.example .env
$ cp tsunagime-api/.env.example tsunagime-api/.env
$ docker compose up -d
$ docker compose exec tsunagime-api bash

# inside container
$ composer install
$ ./artisan migrate:fresh --seed 
```