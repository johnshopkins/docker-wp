# Docker WordPress Starter

## Get it running

1. Install [Docker Desktop](https://docs.docker.com/desktop/).
1. Clone this repo:
    ```bash
    git clone git@github.com:johnshopkins/docker-wp-starter.git
    ```
1. Add any themes or plugins needed for the WordPress site to the _./wp-content/themes/_ and _./wp-content/plugins/_ folders in this repo.
1. Replace _dump.sql_ with your site's SQL or keep it as-is (empty) for a fresh installation of WordPress. If you added SQL to _dump.sql_, uncomment line 24 in _compose.yaml_.
1. Build the containers:
    ```bash
    docker compose up -d
    ```
    Note: The WordPress image will automatically install default plugins and themes.
1. Your site is available here: [http://localhost:8080/](http://localhost:8080/). Changes made to files within _wp-content_ will update within the container automatically.

## Connect to the database

* Host: localhost
* Username: admin
* Password: password
* Database: wordpress
