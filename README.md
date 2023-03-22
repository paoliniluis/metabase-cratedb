# Metabase and CrateDB demo

A fully working demo of Metabase connected to CrateDB

## Requirements

Just docker :)

## How to run it

1) clone this repo
2) just type "docker compose up" and everything will be set up for you

## Credentials

username: a@b.com
password: metabot1

If you wish to change that, those are specified in setup/metabase-setup.sh

## Important notes

If you need to test Metabase Pro or Enterprise features, just complete the token in the env var MB_PREMIUM_EMBEDDING_TOKEN in the docker-compose.yml file

If you're using a Mac with ARM processor, you'll see that Metabase initialization is extremely slow. For that you'll need to bundle Metabase in a ARM compatible container like I do here https://github.com/paoliniluis/metabase-arm/blob/main/Dockerfile and then modify the docker-compose.yml as I do here https://github.com/paoliniluis/metabase-arm/blob/main/docker-compose.yaml