# Docker Compose Guide

## What Does the `services:` Block Do?

The `services:` block defines the containers that make up the application. In this mission, it defines two services: `database`, which uses the MariaDB image, and `app`, which uses the Nextcloud image.

## How Does Nextcloud Find the Database?

The `MYSQL_HOST=database` environment variable tells Nextcloud to connect to a database host named `database`. Docker Compose provides service-name-based networking, allowing the Nextcloud container to reach the MariaDB service using that name.

The database connection also requires matching database credentials, including the database name, username, and password.

## Docker Run vs. Docker Compose

The `docker run` command is commonly used to create and run an individual container with options specified on the command line. Docker Compose uses a YAML configuration file to define multiple related services and their settings.

The `docker compose up -d` command starts the services defined in the Compose file in detached mode, allowing them to run in the background.

## Summary

Docker Compose helps cloud engineers define, deploy, and manage multi-container applications consistently. It makes infrastructure easier to reproduce and reduces the need to configure each container manually.
