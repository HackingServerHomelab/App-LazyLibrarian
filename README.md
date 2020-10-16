# App-LazyLibrarian

## Running the Containers

1. Run `./Config/gen_certs.sh` to generate the SSL certificates (alternatively,
   add custom certs to the private folder)
2. Update the `server_name` in [nginx.conf](./Config/nginx.conf)
3. Update the volume mounts in [docker-compose.yml](./Docker/docker-compose.yml)
    * `../Data/config:/config`
    * `../Data/downloads:/downloads`
    * `../Data/books:/books`
4. Run `docker-compose -f ./Docker/docker-compose.yml up -d`

## First Time Setup

1. Visit <https://your-ip>
2. Configure LazyLibrarian as you see fit
