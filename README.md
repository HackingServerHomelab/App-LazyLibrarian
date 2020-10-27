# App-LazyLibrarian

## First Time Prerequisites

1. Run [Traefik](https://github.com/mattlombana/App-Traefik)

## Running the Containers

1. Update the volume mounts in [docker-compose.yml](./Docker/docker-compose.yml)
    * `../Data/config:/config`
    * `../Data/downloads:/downloads`
    * `../Data/books:/books`
2. Update the Traefik host label in [docker-compose.yml](./Docker/docker-compose.yml)
    * ``"traefik.http.routers.lazylibrarian.rule=Host(`localhost`)"``
3. Run `docker-compose -f ./Docker/docker-compose.yml up -d`

## First Time Setup

1. Visit <https://your-ip>
2. Configure LazyLibrarian as you see fit
