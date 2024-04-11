
This repository creates a docker container for kPlaylist. Find the main repo here: [dysproseum/kplaylist-php7](https://github.com/dysproseum/kplaylist-php7).

## Setup instructions

Clone the kplaylist webroot:
```
git submodule init
git submodule update --recursive --remote
```

Build the docker image:
```
docker-compose build
docker-compose up -d
```

Visit http://localhost/kplaylist-php7

On the kPlaylist installer page, select the "Use existing database" option.

When installation completes, refresh the page and log in:

```
Username: admin
Password: admin
```

## Configuration:

Set the media path:

1. Click on the Admin Control -> Settings button
2. On the "File handling" tab, set the "Base directory" to `/media/`
3. Click "Save" and click "Close"

Update media database:

1. Click on the Admin Control -> Update button
2. Click "Update"
3. After the update finishes, click "Close"
4. Refresh the page

The docker-compose configuration was based off of [sprintcube/docker-compose-lamp](https://github.com/sprintcube/docker-compose-lamp).
