
This repository creates a docker container for kPlaylist. Find the main repo here: [dysproseum/kplaylist-php7](https://github.com/dysproseum/kplaylist-php7).

## Setup instructions

Clone the kplaylist webroot
```
git submodule init
git submodule update --recursive --remote
```

Build the docker image
```
docker-compose build
docker-compose up -d
```

The docker-compose configuration was based off of [sprintcube/docker-compose-lamp](https://github.com/sprintcube/docker-compose-lamp).
