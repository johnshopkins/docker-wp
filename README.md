# Docker WordPress Starter

## Get it running

1. Install [Docker Desktop](https://docs.docker.com/desktop/).
1. Clone this repo:
    ```bash
    git clone git@github.com:johnshopkins/docker-wp-starter.git
    ```
1. Add any themes or plugins needed for the WordPress site to the _./wp-content/themes/_ and _./wp-content/plugins/_ folders in this repo.
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
