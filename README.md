## How to start
```shell
$ cp .env.example .env
$ docker compose up -d
$ docker compose exec tsunagime-api bash

# inside container
$ ./artisan migrate:fresh --seed 
```