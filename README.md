## How to clone
```shell
$ git clone https://github.com/hirokazutoki/tsunagime-dev-env.git tsunagime
$ git clone https://github.com/hirokazutoki/tsunagime-api.git tsunagime/tsunagime-api
$ git clone https://github.com/hirokazutoki/tsunagime-client.git tsunagime/tsunagime-client
$ git clone https://github.com/hirokazutoki/tsunagime-admin.git tsunagime/tsunagime-admin
```

## How to start
```shell
$ cd tsunagime
$ cp .env.example .env
$ cp tsunagime-api/.env.example tsunagime-api/.env
$ cp tsunagime-client/.env.example tsunagime-client/.env
$ cp tsunagime-admin/.env.example tsunagime-admin/.env
$ docker compose up
$ docker compose exec tsunagime-api bash

# inside tsunagime-api container
$ composer install
$ ./artisan migrate:fresh --seed 
```