# Docker WordPress Starter

## Get it running

1. Install [Docker Desktop](https://docs.docker.com/desktop/).
1. Clone this repo:
    ```bash
    git clone git@github.com:johnshopkins/docker-wp-starter.git
    ```
1. Add any themes, plugins, or uploaded files needed for the WordPress site to the _./wp-content/themes/_, _./wp-content/plugins/_, _./wp-content/uploads/_ folders in this repo.
1. Create an _.env_ file based on _.env.example_:
   ```bash
   cp .env.example .env
   ```
1. Open _.env_ and update the database connection settings, as needed.
1. Build the containers:
    ```bash
    docker compose up -d
    ```
    Note: The WordPress image will automatically install default plugins and themes.
1. Optional: Import data into the database. See: [Connect to the database](#connect-to-the-database)
1. Your site is now available here: [http://localhost:8080/](http://localhost:8080/)

## Connect to the database

* Host: `localhost`
* Username: `admin`
* Password: `password`
* Database: `wordpress`

## Helpful commands

* `docker compose down`: Stops and removes the containers and default networks.
* `docker compose down -v`: In addition to removing the containers, volumes are also removed.
* `docker compose down -v --rmi=local`: In addition to removing the containers and volumes, images used by the services are also removed.
